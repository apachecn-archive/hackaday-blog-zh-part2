# 使用电容板的无线电力传输

> 原文：<https://hackaday.com/2015/07/17/wireless-power-transfer-using-capacitive-plates/>

似乎无线电力传输最近很流行。有无线充电垫，特殊的电池组，见鬼，甚至一些手机内置了它！它们都使用感应线圈来传输能量——但如果有其他方法呢？铜线线圈并不总是那么容易放入产品内部…

作为一项实验，【Josh Levine】决定尝试对[电容性电能传输进行概念验证。](http://wp.josh.com/2015/07/11/the-other-way-to-do-wireless-power-capacitive-power-transmision-proof-of-concept/)

他首先演示了使用两个铜线线圈给 LED 供电的感应电能传输。充电线圈的峰峰值为 15V，频率为 1MHz，这是电感充电的一个相当典型的值。然后他给我们看了两个贴着锡纸的玻璃盘子。两个 led 桥接了交替极性的间隙——因为电源是振荡的，所以我们需要一条电子双向流动的路径。没有通过玻璃连接，但当它放在充电板上时，led 就会亮起。充电板以 5MHz 的频率提供 30V 峰峰值电压。

它使用[电容耦合](https://en.wikipedia.org/wiki/Wireless_power#Capacitive_coupling)或静电感应的概念工作。它没有像感应电能传输那样广泛使用的主要原因是因为它需要更高的电压来传输大量的电能——这可能是危险的！但有一件好事是，它不会造成太多的干扰，因为磁场很大程度上被限制在两个板块之间。

[https://www.youtube.com/embed/IXZjVLFIIcM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/IXZjVLFIIcM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

现在这只是第一部分，[Josh]正计划继续研究这个问题，看看他是否能创建一个实用的系统——我们将随时向您报告！

我们想知道无线电力传输的下一件大事会是什么？下一辆特斯拉汽车会在你的车道上无线充电吗？或者可能是[四轴飞行器的充电垫？](http://hackaday.com/2014/01/01/wireless-power-transfer-for-quadrotors/)