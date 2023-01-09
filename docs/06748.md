# THP 入门:带 VGA 和 NTSC 的 CPLD 视频卡

> 原文：<https://hackaday.com/2014/08/06/thp-entry-cpld-video-card-with-vga-and-ntsc/>

![NTSC](img/562a903977f4a3fe89dce0914c85c3c2.png)

[PK]正在做一个非常简单的显卡，打算用便宜的 CPLD 输出 640×480 VGA。该接口将是 5 伏 SPI，这意味着对于任何想要在微控制器项目中放置合理(且便宜)显示器的人来说，这里有巨大的潜力。该项目已经取得了很大进展，他的最新更新展示了以前只做过一次的东西:[彩色 NTSC 与可编程逻辑](http://hackaday.io/project/1943)

这套设备的大脑是来自 Xilinx 的 5100 针 CPLD。除此之外，其余的组件是一个晶体，锁相环，和一个几乎热闹的 R2R 阶梯电阻数量。一个特别独特的元件是 25.056815 MHz 晶体，乘以 2，它的速度足以驱动 VGA 显示器。将晶体除以 7，得到 NTSC 色同步信号频率所需的 3.579545 MHz。这是 VGA 和 NTSC 在一个单一的可编程逻辑项目，这是我们能找到的一个 FPGA 项目，而彩色 NTSC 却无法管理。

项目的下一步是设计 PCB 并计算出帧缓冲器的代码。[PK]放个演示展示一下 VGA 和 NTSC 都有；你可以看看下面。

* * *

![SpaceWrencher](img/4892437613088ab3882681a2ec04a2bb.png) **本帖介绍的项目是[黑客大奖](http://hackaday.io/prize)中的一个参赛项目。建造一些令人敬畏的东西，赢得太空之旅或数百个其他奖品。**

[https://www.youtube.com/embed/xUdjdHOkqZE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/xUdjdHOkqZE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)