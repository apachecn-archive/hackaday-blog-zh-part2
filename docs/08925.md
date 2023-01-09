# Hackaday 奖品入口:BS 免费 USB

> 原文：<https://hackaday.com/2015/05/02/hackaday-prize-entry-bs-free-usb/>

看看一些旧的电子杂志，甚至是 10 年前的几篇博客文章，你会注意到一些奇怪的东西:并行端口。那些大的 DB25 是从计算机中取出比特并放入微控制器的方式。这是有原因的:这非常容易做到。

现在，我们要处理 USB，这意味着 VIDs 和 PID、驱动程序、枚举和一大堆 cruft，使 LED 闪烁成为一个令人惊讶的复杂过程。[科林·奥弗林]的 2015 年黑客日项目旨在用[BSU-BS 免费 USB](https://hackaday.io/project/4994-bsu-bs-free-usb) 解决这个问题。

[Colin]使用了几个带有内置 USB 接口的微控制器，而不是连接到另一个微控制器的 USB 转串行芯片。这些芯片加载了固件，并通过计算机端的简单 API 进行控制。如果你想闪烁一个引脚，只需添加一个库到您的项目，并设置引脚高。想在电脑上安装 SPI 吗？这只是设置几个引脚，如 MOSI，MISO 和 SCK，并输入几个字节。这基本上是一个 2 美元的总线盗版，你可以坚持到任何项目。

如果[科林]的名字在 Hackaday 奖的背景下听起来很熟悉，那是因为去年他凭借《ChipWhisperer》获得了第二名。虽然一个小小的 USB 设备并不像破解嵌入式加密的工具那么酷，但 BSU 对全世界数百万硬件修补者来说似乎更有用。

* * *

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)