# 由一段计算历史驱动的非 Arduino

> 原文：<https://hackaday.com/2015/02/17/non-arduino-powered-by-a-piece-of-computing-history/>

有时候，有一些空闲时间是一件幸事，特别是如果你是一个有很多想法和技能将它们付诸实践的黑客。[Matt]很幸运拥有所有这些，最近完成了一个历时 8 个月的雄心勃勃的项目——一个由计算历史巨人英特尔 8086 处理器驱动的[非 Arduino。幸运的是，[Matt]提供了一个链接来描述](http://tech.mattmillman.com/8od/)[非 Arduino 的实际意思是什么](http://en.wikipedia.org/wiki/List_of_Arduino_boards_and_compatible_systems#Non-Arduino_boards)；这是一个与 shield 兼容的板，但与 Arduino IDE 不兼容。

他的动力来自于建造一台老式单板计算机的愿望，特别是一台带有传统本地总线的单板计算机。在早期，用于英特尔新兴微处理器系列的[系统开发套件](http://en.wikipedia.org/wiki/Intel_System_Development_Kit#Intel_SDK-86)会涉及相当多的分立硬件和软件工具，它们都不太容易使用。

回到自己的窝里，[马特]正在努力应对自己的一系列挑战。8086 是一个微处理器，而不是像 AVR 那样的微控制器，所以软件方面的事情是非常不同的。他很快发现自己陷入了复杂概念的困境，比如汇编引导例程、链接器脚本、代码重定位、内存映射、向量等等。硬件方面的事情也很困难。但是他的目标是学习，所以他没有走捷径。

[Matt]详细记录了他的项目，列出了在他的 8OD 板上运行的各种微处理器，描述了使其运行的软件，链接到原理图和源代码。还有一个有趣的部分是关于在 8OD 上运行苏联时期的微处理器克隆。他仍在考虑是否值得大量生产这种电路板，因为它使用了一些不太容易获得的部件。如果你对这个项目感兴趣，你会很幸运。[Matt]有一些备用的原型，他愿意借给任何能够说服他的人，他们可以为项目增加一些价值。

[https://www.youtube.com/embed/UStEvmk3bfM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/UStEvmk3bfM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

谢谢提示，[加勒特]