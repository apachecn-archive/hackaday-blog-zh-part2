# 使用 Ruby 使任何窗口成为布林肯窗口

> 原文：<https://hackaday.com/2015/02/09/use-ruby-to-make-any-window-a-blinken-window/>

[Akhil Stanislavose]想为他的节日橱窗装饰增添趣味。受到闪光灯的启发，他决定让他的前窗具有互动性。[布林肯窗口](https://github.com/akhilstanislavose/blinken-window/blob/master/README.md)是一个由 6×10 个可编程发光二极管组成的网格，运行在树莓派上。由于 RasPi 没有足够的 GPIO 引脚用于 60 个 led，因此[Akhil]使用 8 个菊花链标准 CD4094(也可以使用 74HC595)移位寄存器构建了一个扩展板来容纳它们。

[Akhil]设计了一个 PCB 来代替扩展板以备将来使用。它本质上是模块化的，因此它们中的许多可以连接在一起，以提供所需的输出，允许任何大小的窗口成为布林肯窗口。PCB 仍在制造中，但 [Eagle 文件可供下载](http://goo.gl/GG7Nz7) (zip 文件)。Ruby 用于实现 API。你可以在 [GitHub](https://github.com/akhilstanislavose/blinken-window) 上找到项目文件，它也有[的一个模拟器](https://asciinema.org/u/7916)，你可以在你的电脑上运行它，看看一个动画或游戏最终会如何出现在窗口上。在演示视频中，[Akhil]演示了如何使用智能手机作为控制器，使用布林肯窗口播放 Pong 版本。[Akhil]还提供了一些可以扩展的基本动画示例。我们很乐意看到俄罗斯方块的实现。有这么多有趣的方法可以将常规窗户变成动态显示器，我们开始轻蔑地看着我们自己的懒惰、漏风的窗户。

休息之后，请观看布林肯之窗的运行。

[https://www.youtube.com/embed/FQo2XVC0iSQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/FQo2XVC0iSQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)