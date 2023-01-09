# TI 发射台的冰电子管钟

> 原文：<https://hackaday.com/2012/09/17/an-ice-tube-clock-for-the-ti-launchpad/>

![](img/7cc3587c9d67926b8664373833bb525e.png "iceman")

因为 Nixies、Decatrons 和 VFD 管真的很酷，43oh 论坛[上的【cubeberg】为 TI Launchpad](http://www.43oh.com/forum/viewtopic.php?f=35&t=3105) 设计了一个 IV-18 时钟。

和 adafruit 的[冰电子管时钟](http://www.ladyada.net/make/icetube/)一样，【cubeberg】的项目使用了一个俄罗斯的 IV-18 VFD 电子管，可以方便地从易贝获得。在板上，有三个按钮用于改变时间和设置闹钟，还有一个 [MAX6921](http://www.maximintegrated.com/datasheet/index.mvp/id/4097) VFD 管驱动器和一个小型开关调节器，用于将发射台的 5 伏电压提高到电子管要求的 50 伏。

[cubeberg]的 PCB 设计上还留有一点空间，他用蜂鸣器和温度传感器的接头填充了这个空间。目前，代码不支持报警功能，他仍在等待一些元件来完成电路板的温度计部分，但这仍然是一个非常好的时钟的制作。

如果你想拥有自己的 Launchpad ice tube 时钟，[bluehash]正在为 430h 论坛成员组织一次团购。如果他们能制造出 15 件，这款钟的单价将低于 5 美元。非常酷，而且非常便宜，当你想到 TI 实际上是在赠送发射台。