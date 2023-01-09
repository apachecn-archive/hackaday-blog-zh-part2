# 适用于 Mac Plus 的可重写 ROM

> 原文：<https://hackaday.com/2014/12/23/rewritable-rom-for-the-mac-plus/>

Macintosh Classic 是一款 9 英寸单色屏幕的小型一体机，是苹果发布的最有趣的机器之一。这是该公司第一次尝试低价电脑，也是第一台售价低于 1000 美元的麦金塔电脑。发布于 1990 年，其功能列表与四年前发布的 Macintosh Plus 几乎相同。Classic 还有一个有趣的功能，这是其他任何 Mac 都没有的。它可以通过在启动过程中按住一系列键来启动完整的操作系统，在本例中为 System 6.0.3。这使它成为一个特殊的无盘工作站。它很便宜，你真正需要的是一个 1.44 兆软盘上的文字处理器或电子表格程序来做真正的工作。

大混乱电线公司的史蒂夫和 80 年代末的苹果工程师有着相同的想法。拿一台 Macintosh Plus，给它多一点内存，装一个操作系统。(史蒂夫)走得比那些苹果工程师想象的要远一些。他为 Mac Plus 制作了一个可重写的 ROM 盘，将这台古老的电脑变成了一个完全可配置的无盘工作站。

构建用填充了 29F040B 闪存芯片的适配器板替换了两个库存 ROM 芯片。它们正是你所期待的——装载了 Flash 而不是稍微更难重新编程的 EEPROM 的巨大老式 PDIPs。由于额外的空间，两个额外的电线需要连接到中央处理器。其结果是，在一台普通可移动磁盘驱动器容量只有 800kB 的计算机上，启动时 Macintosh 可以使用整整一兆字节的闪存。

用于在 Mac Plus [中填充这些闪存芯片的硬件适配器由【Rob Braun】](http://synack.net/~bbraun/plusrom/index.html)制造，而这一构建的软件部分来自【Rob】和【Doug Brown】。他们研究了 Macintosh Classic 的 ROM 磁盘驱动程序是如何工作的，[【罗布·布劳恩】开发了一个独立的 ROM 磁盘驱动程序](http://synack.net/~bbraun/macromboot.html)，带有一个新的海盗主题的启动图标。[史蒂夫]然后挖掘并在 Metrowerks Codewarrior 中创建了一个老派的 Mac 应用程序，向 ROM 写入新的值。从 Shufflepuck 到 Glider，再到 System 7.1 的副本，任何东西都可以放在这个 rom 盘上。

这不是我们第一次看到旧 MAC 电脑的 ROM 启动盘。在旧的 Mac II 系列电脑中有很多空闲的地址空间，并且[【道格·布朗】找到了一个很好的用途](http://www.downtowndougbrown.com/programmable-mac-rom-simms/)。这些旧计算机中有些有可选的 ROM SIMM。你可以在为 ROM 保留的地址空间中放置多达 8 兆字节，使用类似的 ROM 磁盘驱动程序，[道格]可以将整个系统放在 ROM 中，或者[使启动时钟异常长](https://www.youtube.com/watch?v=Yen0omvBo2Y)。