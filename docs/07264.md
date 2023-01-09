# 黑客日十周年:非二进制计算

> 原文：<https://hackaday.com/2014/10/07/hackaday-10th-anniversary-non-binary-computing/>

[https://www.youtube.com/embed/TFTK074nG_M?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/TFTK074nG_M?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

当[Thundersqueak]为 Hackaday 奖寻找项目时，她知道这需要是一个特殊的项目。物联网设备和微控制器是一回事，但它并不能真正让你脱颖而出。不，她的项目需要例外，她转向了[逻辑和平衡三进制计算](http://hackaday.io/project/1043-Base-3--Ternary-Computer-from-scratch.)。

[Thundersqueak]从一些非常有趣且几乎不为人知的历史计算设备中获得灵感，设计了她的三进制计算机。第一台是托马斯·福勒机器，早在 1838 年就设计好了。使用平衡的三重机械装置，它可以数到几千。福勒机器被用来计算日志，以及当时常见的枯燥的数学任务。

更多的研究发现了 Setun，这是 1958 年由真空管制成的电子计算机。这台计算机可以用 18 个三进制数字数到 387，000，000。在你现在使用的二进制机器上，表示它需要 29 个二进制数字。这是一种效率提高 2.5 倍的构建计算机的方式，当你在 20 世纪 50 年代的苏联寻找合适的真空管时，这是一个伟大的想法。

[雷霆之声]不是在和真空管打交道——她对半导体世界了如指掌。在为三值逻辑构建了一些真值表之后，她开始设计电路来满足这台计算机应该做的事情的要求。该设计使用分离式供电轨——负电压、正电压和地，第一个原型电源由 741 运算放大器制成。从那里，它只是试验板的东西，检查她的门，晶体管和真值表，开始创建她的三进制计算机。

三进制计算机的基本构件完成后，[雷霆之声]开始设计基本的 ALU。从半加法器开始，该设计扩展到具有纹波进位的全加器。我们确信有倍增、旋转和其他一切将这个项目变成 CPU 的计划。