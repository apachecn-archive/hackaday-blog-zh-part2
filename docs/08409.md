# 用工业控制单元构建工业控制单元

> 原文：<https://hackaday.com/2015/02/26/building-an-industrial-control-unit-with-an-industrial-control-unit/>

早在 70 年代，工业控制是通过继电器和梯形逻辑或新的可编程逻辑控制器来实现的。这些设备打开和关闭开关，在工厂内移动物品，并保持整个运作顺利进行。在 70 年代末，摩托罗拉推出了一种塞入微型芯片的工业控制装置。芯片 MC14500 让尼古拉着迷。他最终用这个芯片建造了一个重症监护室，尽管这是 30 年前的标准做法，但它仍然是一个有趣的建造。

[Nicola]的 ICU 非常简单，只有 8 个继电器、8 个输入、MC14500、一个时钟和一些 ROM。连接好电路后，[Nicola]编写了一个编译器，尽管这个芯片非常简单，但手动将操作码写入 ROM 也不是不可能的。

为了演示他的 ICU，[Nicola]连接了一个开/关开关、一个开始按钮和一个停止按钮。输出为黄色、绿色和红色灯。即使对于基于继电器的控制方案来说，这也是一项简单的任务，但[Nicola]的电路板做任何事情都不会出现故障。

如果你在寻找稍微复杂一点的东西，我们看到[MC 14500 去年被用作几乎 CPU](http://hackaday.com/2014/04/20/the-computer-without-a-cpu/)。

下面视频。

[https://www.youtube.com/embed/2l-q3JkEEqE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/2l-q3JkEEqE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)