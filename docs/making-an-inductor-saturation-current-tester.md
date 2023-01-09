# 制作电感饱和电流测试仪

> 原文：<https://hackaday.com/2014/09/23/making-an-inductor-saturation-current-tester/>

[卡勒]向我们透露了他在几个晚上做的一个快速项目:[一个电感饱和电流测试仪](http://www.dgkelectronics.com/quick-project-inductor-saturation-current-tester/)。用于它的所有元件都是从一个强大的电信电源中抢救出来的，它允许测试仪在 30 微秒内在待表征的电感器中运行高达 100A 的电流。

在设计开关模式电源(SMPS)时，了解电感的极限非常方便，因为不适当的选择可能会导致高负载下的性能非常差。[卡勒]的测试器只是一个 N-Mosfet 开关电源通过一个负载，而分流允许电流测量。当流经电感的电流突然达到峰值时，就可以找到饱和点。从上图可以看出，16 个 4700uF 电解电容用于补偿 Mosfet 激活时的突然压降。在休息之后嵌入了该系统运行的视频。

[https://www.youtube.com/embed/FjLfrrwpjBs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/FjLfrrwpjBs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)