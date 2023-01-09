# 分析微软 Surface Touch 键盘盖

> 原文：<https://hackaday.com/2015/08/15/analyzing-the-microsoft-surface-touch-keyboard-cover/>

微软 Surface 是一款非常棒的平板电脑，但它有一个问题:只有一个 USB 端口。不过，还有一个额外的端口:Surface Touch 键盘连接器的连接器。这就是【Edward Shin】正在[研究](http://edwardsh.in/keyboard%20cover/2015/08/13/applying-logic-to-the-surface-touch-cover/)的目的，他的长期目标是创造一种适配器，让他能够将 Thinkpad 键盘连接到这种专有连接器上。他在[的最初工作](http://edwardsh.in/keyboard%20cover/2015/02/23/probing-a-surface-touch-cover/)确定该连接器使用微软自己的[I2C HID 协议](https://msdn.microsoft.com/en-us/library/windows/hardware/Dn642101.aspx)，该协议通过 I2C 连接发送标准 USB HID 协议。到目前为止还不错，但之后似乎有点奇怪，串行连接以近 1 Mbps 的速度运行，每次传输发送 9 位，1 位停止。据推测，这是因为[微软曾计划发布使用这种连接器](http://www.theverge.com/2013/9/24/4765048/can-microsofts-futuristic-blade-accessories-give-the-surface-the-edge)的其他设备，但目前为止还没有结果。

有人想帮他吗？他发布了一些从连接中捕获的数据进行分析，并寻求帮助。我们希望他能制造出自己的转换器:一台配有像样键盘和开放 USB 端口的微软 Surface 将是一个很好的便携式设备。额外收获:对于那些喜欢拆键盘的人来说，他拆了一个很棒的[触摸键盘，揭示了一些有趣的东西](http://edwardsh.in/cover/2014/10/19/microsoft-touch-cover-mini-teardown/)，包括许多标记良好的测试点。

Via [ [Reddit](https://www.reddit.com/r/Surface/comments/3gv0j6/applying_a_logic_analyzer_to_the_surface_touch/)