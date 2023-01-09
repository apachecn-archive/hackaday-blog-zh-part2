# 在英特尔爱迪生上运行毁灭

> 原文：<https://hackaday.com/2015/01/10/running-doom-on-the-intel-edison/>

几个月前，Intel Edison 发布，承诺将完整的 x86 系统放在 SD 卡大小的主板上。这不可避免地导致了与其他基于 ARM 的单板计算机的比较，以及爱迪生在 0.100 英寸网格上没有视频输出、以太网或 GPIO 引脚的事实。以太网和轻松突破完全是另一回事，但[Lutz] [确实设法给了爱迪生一个适当的显示](http://2ld.de/edidoom/)，使他能够以与当年 486 相同的速度运行 Doom。

用于构建的硬件是 Edison、Arduino 分线板、Adafruit 显示器、扬声器和 PS4 控制器。到目前为止，最困难的部分是为爱迪生编写显示驱动程序。这样做的出发点是 [Adafruit 的显示器指南](https://learn.adafruit.com/adafruit-2-dot-8-color-tft-touchscreen-breakout-v2)，但爱迪生的引脚映射被证明是麻烦的。理想情况下，显示应该一次发送 16 位，但分线板上只有 8 位。这并不重要；无论如何，Edison 的单个 32 位内存寄存器中没有 16 个引脚。一次向显示器写入八位的解决方案意味着 Doom 以每秒 15 帧的速度运行。不是很好，但足够玩了。

对于声音，[Lutz]使用 100kHz 的 PWM 运行。它很好用，而且有一个小小的扬声器就足够了。控制是通过蓝牙与 PS4 控制器，设置工作正常。最终结果更多的是概念验证，但很容易看出 Edison 如何作为一个完整的视频、声音和无线网络系统使用。这不是很好，但如果你想要高性能，你可能不会选择 SD 卡大小的主板。

下面是视频演示。

[https://www.youtube.com/embed/jJYpGUOGtDw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/jJYpGUOGtDw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)