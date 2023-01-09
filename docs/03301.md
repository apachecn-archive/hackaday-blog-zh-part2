# 使用 Raspberry Pi 构建的 33 节点 Beowulf 集群

> 原文：<https://hackaday.com/2013/05/21/33-node-beowulf-cluster-built-with-raspberry-pi/>

[Josh Kiepert] [不仅建立了一个 33 节点的 Beowulf 集群](http://coen.boisestate.edu/ece/raspberry-pi/)，而且他确保它看起来令人印象深刻，即使你不知道它是什么。这要归功于他设计蚀刻的配电 PCB。除了通过每个 RPi GPIO 接头注入电力之外，它们还装有一个 RGB LED，在上图中以蓝色亮起。

很久以前，我们看到了 64 节点 RPi 集群。那个用乐高积木作为架子系统来支撑所有的板子。但是[乔希]用支架创造了悬挂在丙烯酸制成的顶板和底板之间的金属柱。每块板的唯一独特之处是 SD 卡，这就是为什么每块板上都有一个标识节点的标签。这些都闪现了几乎相同的图像；主机名和 IP 地址是唯一会从一个变化到下一个的东西。它们已经按物理顺序排列，以便您可以快速找到通过机架的方法。但从功能上来说，这并不重要…将卡放入任何 RPi 中，无论它位于机架中的哪个位置，它都会自动在网络上识别自己。

不要错过[Josh]解释整个设置的演示视频。

[https://www.youtube.com/embed/i_r3z1jYHAc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/i_r3z1jYHAc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)