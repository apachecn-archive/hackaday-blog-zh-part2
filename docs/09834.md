# Arduboy 经典游戏在原始游戏男孩屏幕上播放

> 原文：<https://hackaday.com/2015/08/18/arduboy-classic-plays-on-original-game-boy-screen/>

Arduboy 是一款 Kickstarter 支持的 8 位视频游戏控制台，模仿了一个非常小的任天堂游戏机的外观。Arduboy Classic 实际上使用了经典游戏男孩的外壳、按钮和液晶显示屏。

[uXe]正在使用相同的大脑，一个 ATMEGA32U4，以及一个 328 作为协处理器来处理经典的“creme-n-spinich”game boy 屏幕。2K 的双端口 ram 充当两个微控制器之间的缓冲，这意味着它们不仅可以在彼此不同步的情况下运行，而且每个微控制器可以同时读取或写入 ram。

目前，整个设置是分散在一个试验板上，而所有的接口工作了，但它工作得很好。未来的计划是减少经典游戏系统的主板更换，并且在原有的基础上有足够的空间容纳所有新的电子设备。

如果你不熟悉 Arduboy 项目，看看我们对它的创造者凯文·贝茨的采访。这和[uXe 的]基于该项目的黑客演示都是在休息后发现的。

### 经典显示器上由 Arduboy 提供支持的演示

[https://www.youtube.com/embed/uW2dr-duLH8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/uW2dr-duLH8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

### 阿杜博伊采访[凯文贝茨]

[https://www.youtube.com/embed/FtkQkusqfI8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/FtkQkusqfI8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)