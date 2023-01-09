# Hackaday 奖参赛作品:一个 BeagleBone 逻辑分析仪

> 原文：<https://hackaday.com/2015/05/19/hackaday-prize-entry-a-beaglebone-logic-analyzer/>

如果你有一只猎兔犬，你已经有很多工具了。我们已经看到它们以非常高的帧速率驱动数百个 led，用作古代计算机的显卡，以及软件定义的无线电。为了获得 Hackaday 奖，[Kumar] [将他的 BeagleBone 变成了一个 14 通道、100Msps 的逻辑分析仪](https://hackaday.io/project/4395-beaglelogic)，足以调试你正在进行的所有业余电子项目。

BeagleBone 作为逻辑分析仪只能有这种性能，因为它的 pru，这些花哨的外围设备使 Beagle 非常擅长快速闪烁引脚。[Kumar]在这个项目中使用了 BeagleBone 中的两个 pru。PRU1 从输入探针读取，PRU0 将所有样本直接写入 DDR 存储器。从那里开始，样本就被放到内核模块和应用程序中，无论是 sigrok、dd，还是您用 Python 编写的东西。

与我们今天拥有的 Salae Logic 和 DSLogic 等廉价逻辑分析仪相比，[Kumar]的项目与任何商业产品一样好(前提是你可以接受 14 个通道而不是 16 个)，并且因为它基于 BeagleBone，所以该软件可以无限扩展。

更新:在这篇文章写完但发表之前，[Kumar] f [完成了一篇关于他如何用 BeagleBone 的 PRUs](http://theembeddedkitchen.net/beaglelogic-building-a-logic-analyzer-with-the-prus-part-1/449) 构建逻辑分析器的博文。这是一个真正的教程，有足够的代码演示，允许任何人在 BeagleBone 上构建自己的 8 位分析器，并且还会有更多的更新。

* * *

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)