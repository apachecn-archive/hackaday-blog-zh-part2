# 16FUSB —它类似于 PIC 16F628 的 V-USB

> 原文：<https://hackaday.com/2012/05/07/16fusb-its-like-v-usb-for-the-pic-16f628/>

![](img/884e2fa8368e462b73c3a20dc42dfe6a.png "16fusb")

如果你有一个相当简单的 USB 设备的想法，但不想投资在更昂贵的微控制器上，这个库会让你感兴趣。它是 PIC 16F628 的[低速 USB 协议的软件实现。你可以花大约 2 美元买到这些，只需要一些其他元件就可以完成电路。嘿，你甚至不需要一个合适的 PIC 程序员来刷新代码。这是同一个芯片](http://www.lendlocus.com/?q=16fusb)[我们刚刚看到一个 Arduino 充当程序员](http://hackaday.com/2012/05/02/arduino-can-program-pic-too/)。

电路设计看起来与 V-USB 堆栈完全相同，后者为低端 AVR 微控制器提供 USB 功能。除了芯片，你还需要一个晶体振荡器、几个 3.6V 齐纳二极管和一些无源元件。设计中有几个 led，但我们认为这些是反馈用的，对电路的功能并不重要。

项目帖子中包含了大量的数据，所以你可以把它收藏起来以备后用。