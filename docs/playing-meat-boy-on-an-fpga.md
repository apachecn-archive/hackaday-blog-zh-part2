# 在 FPGA 上玩人肉男孩

> 原文：<https://hackaday.com/2013/03/26/playing-meat-boy-on-an-fpga/>

我们通常会看着这些 FPGA 大学项目，并思考为这项工作获得荣誉该有多有趣。但在这种情况下，我们无法想象在 FPGA 中实现“肉食男孩”的游戏机制会有多困难。休息后看看它在剪辑中的表现。

请记住，对于 FPGA，您基本上是通过使用代码来构建硬件设备。该项目的 Reddit 讨论为从哪里开始提供了一些线索(甚至[也分享了源代码](https://github.com/alteraMeatBoy/AlteraMeatBoyHD))。Altera DE2 使用 60Hz 的 SXGA 将游戏推送到显示器上。地图布局为 32×32 个图块的集合，每个图块在内存中用 2 位表示。[SkipToThe3nd]确实详细介绍了物理学是如何工作的，但是我们甚至不能开始解释讨论的这一部分。

在这里被克隆的游戏是肉仔，超级肉仔的前身。如果你从未听说过这个游戏，我们建议你去看 *[独立游戏:电影](http://buy.indiegamethemovie.com/)，*这部纪录片讲述了几个独立游戏开发者试图将他们的游戏推向市场的故事。

[https://www.youtube.com/embed/ak7hbttVyVk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ak7hbttVyVk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)