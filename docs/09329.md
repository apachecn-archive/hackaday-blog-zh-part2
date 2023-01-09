# Hackaday 奖参赛作品:HOMER，一款用于微控制器的 2D GPU

> 原文：<https://hackaday.com/2015/06/19/hackaday-prize-entry-homer-a-2d-gpu-for-microcontrollers/>

用微控制器做的最难的事情就是视频。时序必须精确，即使是低分辨率的视频也需要相对较大的内存，而微控制器通常没有这么多内存。HDMI？这就进入了微控制器向导的领域。

尽管有这些限制，[monnoliv] [正在为微控制器](https://hackaday.io/project/5651-homer)开发 GPU。它通过 HDMI 输出 1280×720，具有 24 位调色板和 2D 硬件加速。

这是一个非常有趣的项目。通常，如果你想在一个项目中使用图形和显示器，你会看到一个 Linux 系统，以及所有的二进制 blobs 和封闭的源代码驱动程序。【monnoliv】的 HOMER 显卡不需要 Linux，也不需要非常高性能的微控制器。它只是一个简单的 SPI 设备，带有一堆存储器和一个 FPGA，可以将最小型的微控制器变成一台可以输出全高清图形的机器。

这不是 Hackaday 奖中唯一的微控制器开源显卡；就在几天前，我们看到了另一款用于微控制器的 SPI 控制显卡 [VGAtonic](http://hackaday.com/2015/06/15/hackaday-prize-entry-an-open-source-graphics-card/) ，这次输出的是 VGA 而不是 HDMI。这两个都是优秀的项目，如果其中一个投入生产，它们都很便宜:都不到 100 美元。如果你想在不求助于 Linux 的情况下玩高分辨率视频，这正是你想要的。

* * *

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)