# 神经网络和 MarI/O

> 原文：<https://hackaday.com/2015/06/14/neural-networks-and-mario/>

《我的世界》巫师，超级马里奥世界纪录保持者 speedrun【SethBling】[正在试验机器学习](https://www.youtube.com/watch?v=qv6UVOQ0F44)。他建立了一个程序，将使用神经网络和遗传算法让马里奥通过整个级别的*超级马里奥世界*——甜甜圈平原 1。

神经网络只是接受一个输入，在这种情况下，一个代表它正在玩的游戏中的精灵的小图形，通过一系列人工神经元发送该输入，并将其转化为控制器的命令。这是一个极其简单的神经网络——能让马里奥通过整个关卡的网络不到十几个神经元——但经过足够的训练，即使简单的网络也能完成非常复杂的任务。

为了训练网络，或者对输入、神经元和输出之间的连接进行加权，[SethBling]正在使用一种进化算法。该算法首先生成几个随机的神经网络，观察马里奥在甜甜圈平原 1 上的进展，并为每个网络分配一个适应值。每一代中最好的网络被组合起来，这个过程继续到下一代。MarI/O 花了 34 代才可以不死的完成关卡。

互联网花生画廊的一些成员指出[汤姆·墨菲的一篇论文/YouTube 视频](https://www.youtube.com/watch?v=xOCurBYI_gY)概括了一种完全不同的技术来玩一大堆不同的 NES 游戏。虽然[塞思布林]和[汤姆·墨菲]的算法都使用某些变量来决定自己的成功与否，但[汤姆·墨菲]的技术几乎是自动运行的；它将像它被给予的训练数据一样发挥作用。[SethBling]的算法不需要训练数据——这就是使用遗传算法的全部意义。

[https://www.youtube.com/embed/qv6UVOQ0F44?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/qv6UVOQ0F44?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/xOCurBYI_gY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/xOCurBYI_gY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)