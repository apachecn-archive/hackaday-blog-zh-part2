# 黑客日 10 周年:乔恩·麦克法伦和螺旋桨

> 原文：<https://hackaday.com/2014/10/10/hackaday-10th-anniversary-jon-mcphalen-and-the-propeller/>

[https://www.youtube.com/embed/QQ3XbMYcZiw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/QQ3XbMYcZiw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[Jon]来到我们的 10 周年纪念迷你会议上谈论推进器，从他的简短介绍来看，他的黑客信誉正在飙升。他有一个关于 IMDb 的网页，他的第一台电脑是 T2 的 COSMAC。大约在 1993 年，他听说一家小公司推出了 BASIC Stamp，和我们一样，他也不相信这种新技术能像宣传的那样发挥作用。不过，他尝试了一下，在那之后的几年里，他每天都在设计基本邮票。

在他的腰带下有许多闪烁的光项目，[Jon]总是与中断作斗争，想办法让 LED*准确地在他想要它闪烁的时候闪烁。自 1993 年以来，Parallax 发生了很多变化，现在他们正在与 Propeller 一起工作，这是一款 8 核微控制器，中断已经成为过去。他展示了一只来自*英雄联盟*的巨大的 10 英尺高的熊，全部由一个螺旋桨控制，使用 1000 个发光二极管看起来像火和火焰。*

[Jon]分享了推进器的架构，这个微小的塑料封装的硅片内部是野生的；它是八个 32 位微控制器，共享一些 ROM 和 RAM，由一个叫做 Cog 的东西控制，让每个微控制器访问地址、数据和 IO 引脚。

当螺旋桨第一次发布时，有几个关于芯片如何编程的问题。c 并不适合多核工作，所以 Parallax 想出了一种叫做 Spin 的语言。它是为多核微控制器编写的，从[Jon]在 demo hell 的小会议来看，它并不比 Python 难学多少。还记得您学习 Python 语法的那一两个小时吗？是啊，学习旋转不是一个巨大的时间投资。

尽管你可以用 C 和 C++ 编写螺旋桨程序，但 Spin 成为螺旋桨的官方语言是有原因的。它甚至没有那么难，如果你想尝试多核微控制器编程，Propeller 就是一个好方法。[这也是一款开源芯片](http://hackaday.com/2014/08/07/parallax-propeller-1-goes-open-source/)，所以你可以用 FPGA 板试试。