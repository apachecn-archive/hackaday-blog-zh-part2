# Hackaday 奖参赛作品:一款开源显卡

> 原文：<https://hackaday.com/2015/06/15/hackaday-prize-entry-an-open-source-graphics-card/>

对于去年的 Hackaday 奖，[PK]试图为微控制器和无头 Linux 系统构建一个显卡。它只有 640×480 分辨率的 VGA，但整个项目是围绕通过 SPI 与微控制器通信的 CPLD 设计的。[PK]自己也承认，这次获奖是一次失败。已经很晚了，但是现在他有整整一年的时间来完善他的设计。这意味着他可以参加 Hackaday 奖的第二版 VGATonic 。

VGATonic 版本 2 使用 Xilinx XC95144XL CPLD 进行 VGA 时序控制，并使用 ATTiny 2313a 读取 SPI 总线。显存是 4 兆位的静态 RAM。这几乎是最基本的 VGA 显卡所需的全部，所有这些都封装在一个 3×3 英寸的 PCB 上。

以 25FPS 运行的 640×480 8 位图形可以做很多事情。在下面的视频中，[PK]有一个各种各样的“hello world”，Doom，运行在一个带有 SPI 显卡的 Raspberry Pi 2 上。对，是树莓派的显卡，看起来真的很不错。

设计的进一步改进将包括一些原始的图形程序。不是 OpenGL 或任何花哨的东西，只是为了减少 SPI 总线上的写入次数。这是一个伟大的项目，如果您想将视频添加到英特尔 Galileo 或其他微控制器项目中，这是一个完美的选择。[PK]有一个视频演示，你可以在下面看看。

* * *

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)

[https://www.youtube.com/embed/qo9iJGTwuEo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/qo9iJGTwuEo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)