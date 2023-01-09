# DIY NES 控制器不改变设计

> 原文：<https://hackaday.com/2013/01/28/diy-nes-controller-makes-no-changes-to-the-design/>

我们喜欢这个项目，因为它非常简单。毕竟，为现代游戏系统重建控制器中的硬件几乎是不可能的。[Guillermo A. Amaral B.]有一堆零件闲着，决定在[试一试，再造一个原始的任天堂娱乐系统控制器](http://guillermoamaral.com/read/custom-nes-controller/)。

如果你不熟悉这个品牌的复古游戏硬件内部的电子设备，你可能会惊讶地发现，几乎没有任何逻辑硬件。电路板中间的芯片是一个 4021 并行到串行移位寄存器。它连接到按钮，并使用来自电缆的时钟信号通过串行线脉冲输出按钮状态。所以[Guillermo]所做的就是把芯片和每个按钮连接起来。

在上面的图像中，他的拇指挡住了用于方向控制和选择的 5 向开关(点击中键)。黄色和绿色按钮充当 A 和 B，由于他的棋盘布局中的一个错误，开始按钮位于棋盘的另一侧。他确实对此有一些未来的计划。他正在做一个 Raspberry Pi 项目，该项目将监控和记录控制器串行数据，以便您可以回放它。听起来像电子游戏用的钢琴。

想看看这个的小版本吗？几个月前，一个更小的封装中的相同硬件被组装在一起，以构建世界上最小的 NES 控制器。

[途径 [Adafruit](http://www.adafruit.com/blog/2013/01/21/custom-nes-controller-as-seen-on-adafruit-show-tell/)