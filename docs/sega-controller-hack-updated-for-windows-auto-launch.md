# 世嘉控制器黑客更新 Windows 自动启动

> 原文：<https://hackaday.com/2015/01/03/sega-controller-hack-updated-for-windows-auto-launch/>

谁知道现代版本的 Windows 已经取消了插入 u 盘时自动启动的选项？没什么大不了的，除非像[sonicdude10]一样，你想把黑客攻击建立在行为的基础上。他确实找到了一个变通办法，最近[开发了一个世嘉控制器模拟器，可以在 Windows 电脑上自动播放。](https://www.youtube.com/watch?v=HpJzfOzyKn8)

黑客的大部分灵感来自于几年前他在 Hackaday 上看到的控制器中内置的一个世嘉仿真器。它只是一个类似世嘉的 USB 游戏手柄，内置了一个集线器和拇指驱动器。[sonicdude 10]版本的硬件变化摆脱了旧的拇指驱动器，代之以支持 [U3](http://en.wikipedia.org/wiki/U3) 的驱动器。这是一些 USB 驱动器支持的硬件仿真技巧，允许它们枚举为 CD 驱动器，而不是 USB 大容量存储。在 Windows 中，CD 驱动器的自动播放功能仍然有效。

这些年来，我们对 U3 有所耳闻。早在 2006 年就有一个现已死亡的黑客。我们甚至发现[一条建议将其用于基于 USB 的游戏模拟器](http://hackaday.com/2009/11/19/uzebox-in-an-nes-controller/comment-page-1/#comment-108111)的评论。[sonicdude10]指出了两个有用的工具，让他定制 U3 的执行方式。 [u3_tool](http://u3-tool.sourceforge.net/) 是一个多功能工具，用于调整硬件的行为方式， [u3-autorun](http://sourceforge.net/projects/u3-autorun/) 使自动启动应用程序的定制变得轻而易举。

 [https://www.youtube.com/embed/HpJzfOzyKn8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/HpJzfOzyKn8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)