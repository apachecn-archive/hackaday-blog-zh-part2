# 用袖珍迷你电脑重温 1977 年的尖端电脑

> 原文：<https://hackaday.com/2012/11/06/reliving-1977s-cutting-edge-computer-with-the-pocket-mini-computer/>

![](img/38bdd260f044b4348a064c61079475da.png "chip8")

经典计算机正合[杰夫]的胃口，所以当他为他的袖珍迷你计算机寻找新项目时，他着眼于最早的微型计算机之一:COSMAC VIP，1977 年的 1.76 MHz beast。

COSMAC VIP 是美国无线电公司在 1977 年发布的单板教育计算机。COSMAC 的价格不到 300 美元，比同年发布的臭名昭著的 1300 美元的“水果”电脑便宜得多。为了让年轻的程序员快速上手，COSMAC 与 CHIP-8 编程语言捆绑在一起，使得在屏幕上为所有最终的 PONG 和 Breakout 克隆生成图形变得非常容易。

[杰夫]的 COSMAC VIP 在一台[袖珍迷你电脑](http://propellerpowered.com/shop/?page_id=234)上运行，这是一种非常酷的视差推进器驱动的主板，我们以前见过它模仿其他复古电脑，包括古老的[Commodore SID 合成器](http://hackaday.com/2012/10/18/creating-a-midi-synth-from-a-commodore-sid/)芯片。

因为 COSMAC 的用户界面是非常非常老派的 4×4 十六进制键盘，[Jeff]发现有必要通过焊接自己的 4×4 键盘来模仿这一复古功能。在将 16 个按钮焊接成 8 列 8 行后，[杰夫]将这个键盘连接到一个 [PFC8574a](http://www.ti.com/product/pcf8574a) I2C I/O 扩展器上，并将这个芯片连接到袖珍迷你电脑上的 I2C 总线上。

结果是一个仿真的 COSMAC VIP，它只是乞求一个“微处理器介绍”课程，或者只是一轮俄罗斯方块、井字游戏、月球着陆器，或者这款非常酷的计算机可用的几个突破性克隆之一。一个非常棒的构建，即使它来自计算机时代的黎明。