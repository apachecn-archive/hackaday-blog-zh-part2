# 在硬件中实现的 Zork 虚拟机

> 原文：<https://hackaday.com/2014/11/29/the-zork-virtual-machine-implemented-in-hardware/>

佐克、*银河系漫游指南*以及所有其他 Infocom 文本冒险都比乍看起来要聪明得多。它们实际上运行在一个虚拟机上，游戏文件的所有代码都以 Z-machine 格式存储。如果你正在为十几个平台写游戏，这是很棒的；一旦你在一个系统上运行了一个解释器，整个游戏库就可以运出去了。

虽然 Z-machine 已经被移植到你能想象到的所有逆向计算机和一些不同品牌的微控制器上，但是还没有人在硬件上实现 Z-machine。这是有原因的:太疯狂了。然而，[【Charlie】设法在 FPGA](https://github.com/charcole/Z3) 中实现了 Z-machine，只使用了一些额外的命令来驱动显示器。

该电路由 10 美元的易贝专用 FPGA Cyclone II ep2c 5 构成。除此之外，它只是一些闪光灯，一些内存，一个显示器和一大堆电线。标准的 Z-machine 规范遵循，特别是第 3 版，这意味着这款芯片上的文本冒险可以运行几乎所有的 Infocom 游戏。至少是最受欢迎的。

这不是[Charlie]第一次与 Infocom Z-machine 交战。几年前，他把 Z-machine 移植到了一个奇怪的围栏里。

你可以看看下面[查理]的视频演示。因为 FPGA 中有一点额外的空间，[Charlie]设法把 Mandelbrot 实现和*太空入侵者*作为复活节彩蛋放了进去。

[https://www.youtube.com/embed/HuQZq6DQQDY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/HuQZq6DQQDY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)