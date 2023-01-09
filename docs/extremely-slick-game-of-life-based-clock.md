# 基于时钟的极其光滑的生活游戏

> 原文：<https://hackaday.com/2014/01/11/extremely-slick-game-of-life-based-clock/>

[Matthews]需要一份好礼物送给他的妹夫，他的妹夫恰好是一名数学家和程序员。他想要一些功能强大但同时又让人讨厌的东西，所以他决定尝试制作一款生活时钟游戏。

他最初的灵感来自于我们几个月前分享的一款[游戏《生命之钟》](http://hackaday.com/2013/10/19/game-of-life-clock/)，但做了一些改进。首先，他想要一个更大的比赛场地，所以他找到了一个 16×32 RGB LED 矩阵。其次，他希望时间总是可见的，这样它实际上就像一个功能时钟。

该设备的核心是 Arduino UNO，它利用 Chronodot RTC 模块来精确计时。整个时钟被压克力板包裹着，对于一个自制的项目来说，它看起来非常好。他使用一个名为 [MakerCase](http://makercase.com) 的网站设计了这个箱子，这是一个设计箱子的超级方便的应用程序。

在每一分钟的开始，生命开始了一场新的游戏，它在显示的时间之上进行。顶部的三个按钮允许许多调整，包括亮度，时区，速度，颜色，甚至边缘行为！为了看到它的实际效果，请在休息后留下来。

[https://www.youtube.com/embed/d6uykJIkXng?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/d6uykJIkXng?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)