# 一台精巧的纸板电脑

> 原文：<https://hackaday.com/2014/10/14/a-clever-cardboard-computer/>

早在 70 年代，计算机相当昂贵，大多数人都买不起，贝尔实验室的[David Hagelbarger]设计了 CARDIAC: [纸板辅助计算工具](https://www.cs.drexel.edu/~bls96/museum/cardiac.html)。CARDIAC 是作为一种教育工具而设计的，目的是让没有接触过计算机的人能够学习计算机的工作原理。

心脏计算机是单累加器单地址机器，这意味着指令只在累加器上运行，或者在累加器和一个存储单元上运行。该机器执行 10 条指令，每条指令都分配有一个 3 位十进制操作码。指令集架构包括简单[冯诺依曼](http://en.wikipedia.org/wiki/Von_Neumann_architecture)处理器通用的指令，如加载、存储、加/减和条件分支。

操作计算机相当简单——纸板幻灯片会引导您完成 ALU 和指令解码器的操作，流程图会告诉您下一步该进行哪个阶段。程序计数器由一个纸板瓢虫代表，在每条指令完成后，通过程序存储器手动移动。

尽管 CARDIAC 已经过时并且非常简单，但它仍然是教授微处理器如何工作的有用工具。尽管现代处理器包括多级流水线、微调分支预测器和许多其他改进，但基本的操作原理仍然相同。

喜欢冒险吗？打印出你自己的心脏克隆体，并尝试编写你的第一个纸板计算机程序。

[via [Reddit](http://www.reddit.com/r/programming/comments/2ivo0y/cardiac_a_cardboard_computer_with_only_10/)