# Mill CPU 架构

> 原文：<https://hackaday.com/2013/08/02/the-mill-cpu-architecture/>

基本上有两种计算数据的方法。第一种是 DSP，这是一种对有限的数据集执行非常专业的功能的芯片。这些非常便宜，每瓦特性能惊人，但根本无法进行一般计算。如果你想建造一台通用计算机，你必须使用超标量处理器 x86、PowerPC 或任何其他真正强大的 CPU 架构。超级标量对于通用计算来说是很棒的，但是与 DSP 相比，它们的性能功耗比是很低的。

很多人都研究过这个问题，但什么也没发现。然而，如果开箱即用计算的[Ivan Godard]能够生产出磨坊——对当前 CPU 架构的彻底反思，这种情况可能会改变。

与 DSP 不同，你会在桌面上发现超标量处理器有大量的寄存器，其中大多数是重命名寄存器，或者 CPU 临时存储值的地方。结合这一事实，将数百个这些临时寄存器连接到它们最终将被使用的地方消耗了大约一半的 CPU 功率预算，你就会明白为什么 DSP 比笔记本电脑中的 x86 效率高得多。

[Ivan]对这个问题的解决方案是用一种叫做“带”的东西取代 CPU 中的寄存器——基本上是堆栈和移位寄存器的奇怪组合。CPU 可以从传送带上的任何位置获取数据，执行操作，并将结果放在传送带的前端。任何不用的数据都会从传送带上掉下来；这不是问题，因为 CPU 中使用的大多数数据只使用一次。

理论上，这是一种更有效的通用计算方式。不幸的是，[Ivan]并没有获得工厂的所有专利，所以他的演讲(下面有两个)有点条块分割。尽管如此，这仍然是近年来计算机体系结构中最酷的进步之一，我们希望看到它成为真正的产品。

[https://www.youtube.com/embed/LgLNyMAi-0I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/LgLNyMAi-0I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent) [https://www.youtube.com/embed/QGw-cy0ylCc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/QGw-cy0ylCc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)