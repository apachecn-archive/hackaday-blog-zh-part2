# 定制机械键盘

> 原文：<https://hackaday.com/2014/03/11/custom-mechanical-keyboards/>

[Wyager]正在四处购买一个机械键盘，在注意到定制 PCB 制造的价格大幅下降后，他决定自己制造一个。最终的结果是[一个设计优雅的键盘](http://yager.io/keyboard/keyboard.html)，只要稍加努力，它就可以成为一个非常有趣的 Kickstarter 项目。

该设计有三个要求:便宜，机械开关，非常可定制。廉价的需求通过将键盘分成主/从排列的两部分来解决。这些板通过一个 1/8 英寸的 TRRS 插孔连接，该插孔传送一条 I2C 总线。由于除了在 Teensy dev 板上运行的代码之外，两块电路板完全相同，[Wyager]通过使用他的 OSHPark 订单附带的三块 PCB 中的两块，节省了一些资金。

对于一个失败的项目来说，机械开关——Cherry MX Blues——是相当昂贵的部件。由于担心失败，[Wyager]首先订购了一种只包含一个按键的 PCB。足迹正确后，他升级到 2×2 矩阵。一旦证实了这一点，就订购了 6×5 矩阵。第一次的时候一切都很完美，这是我们很多项目都不能说的。

代码、电路板文件和原理图可从 github 上的[处获得](https://github.com/wyager/micromechboard)