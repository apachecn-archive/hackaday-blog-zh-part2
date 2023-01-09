# THP 半决赛:Theta 打印机

> 原文：<https://hackaday.com/2014/08/28/thp-semifinalist-theta-printer/>

80 年代和 90 年代的早期 3D 打印机以笛卡尔机器人开始，这是 RepRap 项目从最早的开源 3D 打印机设计中得到的启示。过了一会儿，delta 机器人出现了，但这仅仅是在构建板周围移动工具架的一种不同方式。我们还没有真正见过真正的极坐标 3D 打印机，[除了【泰勒安德森】的不可思议的θ打印机](http://hackaday.io/project/812)。

[Tyler]的 theta 打印机旨在打印尽可能多的不同材料，而不会像更传统的打印机那样使用多个工具来减少体积。它将能够在一个巨大的构建体中放置不同颜色的塑料，甚至一些更奇怪的细丝，都在一个单独的打印中。

theta 打印机基于极坐标系统，这意味着不是在 X 和 Y 轴上移动热端，而是构建板在圆周上旋转，挤出机沿着圆周的半径移动。这种旋转的极坐标打印机是我们见过的在打印机上放置多个挤出机的最佳方式，并且还具有作为 3D 扫描仪的伟大平台的额外好处。

有四台挤出机，四台控制每个挤出机位置的电机，一台旋转电机和 Z 轴(如果你数的话，那就是 10 个步进器)，这很可能是 3D 打印机中最大数量的电机。大多数电子板不支持那么多的步进驱动器，而[将](http://reprap.org/wiki/Decapede)的那个不会在 Hackaday 奖结束时准备好。现在，[Tyler]正在运行一个相当标准的 RAMPS 板，并行运行两台挤出机和 R 轴。不过，这对于概念验证来说已经足够好了。

[泰勒]的设计有一个有趣的方面是他可能还没有意识到的:用一张床和四台挤出机，他有效地制造了一台适合大批量生产的 3D 打印机；只需用所有挤压机打印相同的零件，他就能在占地面积与普通打印机相同的情况下，将 3D 打印机的产量翻两番。这听起来可能不多，但当你意识到 Lulzbot 有一个机器人农场生产他们所有的零件时，Theta 打印机开始看起来像一个非常非常好的主意。

下面是[泰勒]的 Theta 视频。

* * *

![SpaceWrencher](img/4892437613088ab3882681a2ec04a2bb.png) **本帖介绍的项目是[入围 Hackaday 奖的半决赛。](http://hackaday.io/list/2864-The-Hackaday-Prize%3A-Semifinalists)**

[https://www.youtube.com/embed/8SplsSDy6So?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/8SplsSDy6So?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/tNpsFQ_VqJ0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/tNpsFQ_VqJ0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/p_tqMAzWGm0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/p_tqMAzWGm0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)