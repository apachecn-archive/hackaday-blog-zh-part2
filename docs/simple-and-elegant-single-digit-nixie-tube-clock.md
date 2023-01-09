# 简洁大方的个位数数码管时钟

> 原文：<https://hackaday.com/2014/12/13/simple-and-elegant-single-digit-nixie-tube-clock/>

我们以前在这里看过一些谢妮的项目，但是这个可能是最简单的。[Pinomelean]设计了这个简单的数码管时钟,只用了很少的元件。

本项目选用的数码管是 IN-12a。这种管子只需 4 美元左右就能买到。它能够一次显示一个数字，从 0 到 9。由于电子管一次只能显示一个数字，时钟被编程为逐个闪烁当前时间的每个数字。每个周期之间有一个较长的停顿，以便更容易判断周期开始和结束的时间。

该系统分为两个主要部分。首先是时钟电路。该时钟由一个带 4MHz 晶振的 PIC 微控制器驱动。所有的逻辑都是通过 PIC 执行的，只需要少量的其他组件。这包括一些电阻和电容以及几个高压 SMD 晶体管来控制数码管。[Pinomelean]提供了这种 PCB 设计，任何人都可以下载并制作自己的时钟。

时钟的第二个组成部分是电源。该系统由锂离子充电电池供电，但[Pinomelean]指出，它也可以通过 USB 供电。对于微控制器来说，较低的电压工作良好，但是数码管需要较高的电压。[Pinomelean]利用从旧的一次性相机中收集的组件建造了自己的高压电源。这种电源板设计也可以下载，但它插入主板，因此如果需要，您可以使用另一种设计..看看下面的演示视频，看看它的实际效果。

[https://www.youtube.com/embed/Vu_8dR9vmck?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Vu_8dR9vmck?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)