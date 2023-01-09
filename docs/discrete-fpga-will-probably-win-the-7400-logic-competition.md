# 分立 FPGA 很可能赢得 7400 逻辑竞赛

> 原文：<https://hackaday.com/2012/11/01/discrete-fpga-will-probably-win-the-7400-logic-competition/>

为了今年的 7400 逻辑竞赛，【尼克】决定用逻辑芯片 ( [互联网档案馆缓存版](http://web.archive.org/web/20150621104100/http://blog.notdot.net/2012/10/Build-your-own-FPGA))构建[一个 FPGA。](http://blog.notdot.net/2012/10/Build-your-own-FPGA)

也许一个简短的解释是为了充分欣赏[尼克]的工作。FPGA 的基本组件是一个片或单元，它对其输入执行布尔运算，并在其输出上发送结果。这些切片的核心是一个查找表——基本上是一个真值表，存储每种可能的输入组合的结果。

实现查找表的一个非常简单的方法是使用 RAM 或 EEPROM 芯片。通过将 EEPROM 的地址线连接到输入端，将数据线连接到输出端，可以非常容易地创建一片 FPGA。

对[Nick]来说不幸的是，74 系列内存早已停产。不过，还有另一个选择:移位寄存器。移位寄存器基本上是一个具有并行输入的 8 位存储器芯片，因此将移位寄存器与 8 输入多路复用器相结合是实现 3 输入 1 输出 FPGA 片的一种非常简单的方法。

在弄清楚如何将这些芯片连接到总线线路后，[尼克]需要一种方法来对它们进行编程。Verilog 或 VHDL 近乎疯狂，所以他编写了自己的硬件描述语言。它当然不如 FPGA 编程的主流解决方案强大，但也绰绰有余。

在休息后的视频中，您可以看到[Nick]在运行密码锁和 PWM 程序时对他的超大型 8 片 FPGA 的概述。所有的代码、原理图和电路板布局都在[Nick]的 git 上，如果你想自己制作的话。


[https://www.youtube.com/embed/7r0CuxFMGBQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/7r0CuxFMGBQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)