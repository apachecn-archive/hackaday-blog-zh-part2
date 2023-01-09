# 将电池电量计添加到零零件项目中

> 原文：<https://hackaday.com/2014/11/08/adding-a-battery-gauge-to-a-project-with-zero-parts/>

检测低电量电池的典型方法是在电路中放入一个比较器，设置它来测量某个阈值电压，然后将该信号发送给微控制器或其它电路，通知某人电池即将耗尽。[【Josh】有一个更简单的方法](http://wp.josh.com/2014/11/06/battery-fuel-guage-with-zero-parts-and-zero-pins-on-avr/)使用一个 8 位 AVR 和零其他部分。

[乔希]使用的芯片是 ATtiny84。该芯片中的 ADC 通常用于测量未知电压与参考电压的比值。[Josh]使用的技巧是反过来做这件事:内部 1.1 伏参考电压是相对于一个未知的标度，即输入电压来测量的。

芯片上 ADC 提供的值始终是 Vin 乘以基准电压的 1024 倍。由于这种情况下 Vin 为 1.1 V，ADC 值已知，因此只需做一些 6 级代数运算即可确定输入电压值。

[Josh]做一个小演示，芯片闪烁显示它从工作台电源接收的电压值。通过闪烁 LED，它可以将 VCC 的当前值闪烁为整数，但是通过使用这种技术，您应该能够获得 VCC 实际上是什么的相当精细的读数。下面视频。

[https://www.youtube.com/embed/oK8oz4Cfu2g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/oK8oz4Cfu2g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)