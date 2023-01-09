# 多色打印头允许 RepRap 打印彩虹

> 原文：<https://hackaday.com/2012/08/27/multicolor-print-head-allows-reprap-to-print-rainbows/>

![](img/2892981fe4f3136bfc083faaba84effd.png "print")

多色 3D 打印机已经出现了一段时间，但大多数这种机器——如 Makerbot Replicator——都存在对齐问题，并且无法即时混合颜色。[RichRap]想出了一个解决这个问题的有趣方法，他让[三个细丝挤出机进入一个热端](http://richrap.blogspot.co.uk/2012/08/3-way-quick-fit-extruder-and-colour.html)，允许他在飞行中改变和混合颜色。

为了印刷多种颜色，[RichRap]开发了一种三挤出机 x 滑架，将彩色细丝发送到一个热端。与 Makerbot 复制器不同的是，[Rich]的挤出机可以将不同的颜色混合并融入印刷品的每一层。

构建的电子部分，[RichRap]用一个斜坡板控制他的打印机的 X、Y 和 Z 轴，但使用一个稍微修改的 Sanguinololu 板作为挤出机马达。挤出机的单个电机驱动器连接到三个拨动开关，允许[RichRap]在运行中切换细丝。

[Rich]有一个非常酷的构造，但这远不是一个完美的解决方案。现在，三种颜色中的任何一种都可以用来打印，但是同时打印两种或三种颜色需要改变固件。我们期待有人在不久的将来解决这个问题，让 CMYK 打印头的圣杯开花结果。

休息之后，您可以看到[RichRap]三色打印头的演示视频。

[https://www.youtube.com/embed/nkkbjpHVNZQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/nkkbjpHVNZQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)