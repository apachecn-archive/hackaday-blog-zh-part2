# 入侵 SD 卡和闪存控制器

> 原文：<https://hackaday.com/2013/12/29/hacking-sd-card-flash-memory-controllers/>

我们希望我们的一些读者目前正在参加今年的[混沌通信大会](http://en.wikipedia.org/wiki/Chaos_Computer_Club)(日程安排可以在[这里](http://events.ccc.de/congress/2013/Fahrplan/schedule.html)和[这里](http://fireglow.de/755/share/30c3-streams.html)找到)，因为许多有趣的会谈正在进行。其中一个解决了[黑客入侵你可能有的所有内存卡中嵌入的内存控制器](http://www.bunniestudios.com/blog/?p=3554)的问题。随着内存存储密度的增加，嵌入式闪存内部的一些扇区更有可能出现故障。因此，所有的制造商都会在他们的卡上添加一个小的微控制器(以及额外的内存),以无形的方式“替换”操作系统中有缺陷的扇区。

[Bunnie]和[xobs]四处购买许多不同的 microSD 卡，以便找到一种可破解的卡。在 30C3 的演讲中(此处为幻灯片)，他们报告了他们对一个特定微控制器品牌 Appotech 及其 AX211/AX215 的发现。通过对他们在网上找到的固件代码进行逆向工程，他们发现了一个简单的“敲击”序列，该序列通过制造商保留的命令传输，使控制器进入固件加载模式。从那里，他们能够逆向工程的 8051 微控制器功能专用寄存器的大部分，使他们能够开发新的应用程序。一些最初的工作是使用基于 FPGA/i.MX6 的平台完成的，该平台由团队开发，名为 [Novena](http://www.bunniestudios.com/blog/?tag=novena) ，我们希望有一天可以购买到它。除其他外，它被用来模拟团队之前移除的闪存芯片。下面是这次演讲的视频。

[https://www.youtube.com/embed/r3GDPwIuRKI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/r3GDPwIuRKI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)