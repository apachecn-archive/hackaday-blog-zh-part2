# THP 参赛作品:由计算器供电的剧院灯光控制器

> 原文：<https://hackaday.com/2014/08/03/thp-entry-a-theatrical-lighting-controller-powered-by-a-calculator/>

![DMX](img/59d4cbff9097c848f87315c7235c79b7.png)

剧院灯光通常在 DMX 的帮助下运行，这是一种基本上是灯光的 MIDI 协议；小巧、轻便、古老，能够在你能想到的最低规格的计算机上运行。对于他的 Hackaday 奖参赛作品，[Alex]认为一个普通的图形计算器足以运行一个完整的 DMX 控制器，在 Arduino 的帮助下，[找到了一种方法来完成它](http://hackaday.io/project/2170)。

该系统的硬件包括一个 TI-84 图形计算器、几个零零碎碎的组件和一个由计算器上的 USB 端口供电的 Arduino Pro Mini。Arduino 使用 [DMXSimple 库](https://code.google.com/p/tinkerit/wiki/DmxSimple)通过 5 针 XLR 插孔处理 250 千波特的 DMX 数据包传输。

运行在计算器上的软件是该项目的新颖部分开始的地方。该软件设计得非常轻便，使用双线链接电缆向 Arduino 发送数据包。DMX 命令使用 TI-83/84 链接协议打包和传输，在 Arduino 上解码，然后发送到照明设备。

虽然这可能不会取代剧院里数千美元的灯光控制台，但它仍然是调试灯光的一个非常方便和便携的工具。这也是[Alex]的第一个电子项目，而且是一个相当不错的项目。

* * *

![SpaceWrencher](img/4892437613088ab3882681a2ec04a2bb.png) **本帖介绍的项目是[黑客大奖](http://hackaday.io/prize)中的一个参赛项目。建造一些令人敬畏的东西，赢得太空之旅或数百个其他奖品。**