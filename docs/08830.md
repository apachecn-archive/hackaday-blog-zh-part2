# VCF·伊斯特:[比尔·赫德]和系统架构

> 原文：<https://hackaday.com/2015/04/20/vcf-east-bil-herd-and-system-architecture/>

上周五的老式电脑节上有十几场讲座，太多了，任何一个人都无法参加。然而，我们确实检查了[【Bil Herd】关于系统架构](https://www.youtube.com/watch?v=D17jmFOUe7g&feature=youtu.be)的演讲，或者他喜欢称之为，通过平衡实现性能的艺术和科学。那是一个小时十五分钟的谈话；咖啡和爆米花协议适用。

本次演讲的重点是如何从头开始设计一个系统，不需要任何假定的硬件或任何特定的外设。这一切都始于一个 CPU、一些内存(无论是哪种类型)和一些 I/O。这就是你所需要的一切，无论你是在设计一台微波炉还是一台超级计算机。

系统的 CPU 可以是任何东西，从简单的 6502，做大量数学运算的向量处理器，或者具有 RISC、流、流水线、SIMD 架构。这个选择将影响使用哪种内存的决定，是静态的还是动态的，是大字节还是小字节。是的，甚至[比尔]还在试图理解字节序。

MMU、I/O 芯片、电传打字机、像 6845 这样的字符显示器，以及 ANTIC、VIC 和 GTIA 在[Bil]提到把整个系统放在一起之前就被削减了。这不仅仅是连接地址和数据引脚并看到整个系统运行的问题。有中断、RTC、总线仲裁、DTACK、RAS 和 CAS 来处理这些问题。这将需要更多的演讲来涵盖，但你可以看到下面上周五的一个。

[https://www.youtube.com/embed/D17jmFOUe7g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/D17jmFOUe7g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)