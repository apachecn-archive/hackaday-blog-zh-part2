# 3D 打印:感应加热

> 原文：<https://hackaday.com/2015/03/15/3d-printering-induction-heating/>

今天，你会发现每一台基于灯丝的 3D 打印机都使用电阻加热器来加热塑料——要么是加热筒，要么是大功率电阻。这很有效率，但也只能做到这一步。考虑到这些加热器只能消耗这么多瓦特，它们只能快速升温。这是一个问题，如果你试图制造一台快速打印机，这也是一个限制。

感应加热器不是将 12 或 24 伏直流电注入电阻加热器，而是将高频交流电通过感应耦合到铁芯的导线。也很有效率，但也很快。不需要高温绝缘，如果设计正确，热质量会更少。塑料快速加热的所有伟大特性。

几年前，RepRap 博客上的[SB]为一个硕士项目设计了一个感应加热器。热端是一个普通的黄铜喷嘴，连接在一个软钢套筒上。叠片铁芯连接到热端，感应线圈缠绕在铁芯上。它的工作，但没有任何真正的进展，把这变成一个适当的喷嘴和热端。毕竟，这只是一个项目。

最后，几年后，[人们从感应加热喷嘴中喷出塑料。[Z]或[Bulent Unalmis]在 RepRap 论坛上发布了一个项目，他正在挤压用感应加热器加热的塑料。这是一个直接驱动系统，在机械上，这是一个比我们现在使用的花哨的热端更简单的系统。](http://forums.reprap.org/read.php?2,481721)

从电子角度来看，要复杂得多。虽然电阻加热器的电子器件只是一个强大的电源和一个 MOSFET，但[Z]使用的是 30 V、160 kHz 的交流电，这是一个很难安装在打印机控制器板上的电路。

这可以被看作是绕过普通控制板的普通 24V 限制的一种方式；把更多的能量注入电阻，它会变得更快。这可能不是热端升温更快的答案，但至少这是一个非常整洁的项目，我们希望看到更多的东西。

下面可以看到[Z]关于他的感应热端的视频演示。谢谢[马特]的提示。

[https://www.youtube.com/embed/PaXcDpXOLYs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/PaXcDpXOLYs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)