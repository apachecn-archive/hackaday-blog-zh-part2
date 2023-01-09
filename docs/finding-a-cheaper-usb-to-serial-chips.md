# 寻找更便宜的 USB 转串行芯片

> 原文：<https://hackaday.com/2014/12/02/finding-a-cheaper-usb-to-serial-chips/>

[FTDI-gate 并不适合任何人](http://hackaday.com/2014/10/22/watch-that-windows-update-ftdi-drivers-are-killing-fake-chips/)，现在随着硬件爱好者和技术修补者放弃最流行的 USB 转串行适配器，一些其他芯片必须填补空白。市场上最便宜的 USB 转串行芯片似乎是 CH340G，在普通零售商那里每个售价 20-40 美分。然而，几乎没有英文文档，CH340 系列的数据手册也不包括该芯片。[【伊恩】来帮你解决](http://fobit.blogspot.com/2014/11/ch340g-in-eagle.html)。他接触了一些这样的芯片，并设法找出了引脚和一些参考原理图。他甚至为你做了一只鹰。这不是很好吗？

CH340 系列芯片完全符合您的预期:全速 USB 设备，模拟标准串行接口，速度从 50bps 到 2Mpbs。芯片支持 5V 和 3.3V，所有怪异的 modem 线都支持。这种芯片甚至有一个 IrDA 模式，因为在 90 年代，无线通信就像你记忆中的一样快。

在[Ian]的帮助下，我们现在有了 USB 转串行芯片的廉价来源。如果你需要数据手册，[给你](http://www.seeedstudio.com/wiimg/7/7c/CH340DS1_EN.PDF)。驱动程序有点难找，但你要找的是 *CH341* 系列芯片。用一点谷歌搜索就能找到。