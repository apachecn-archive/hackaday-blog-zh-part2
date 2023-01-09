# 捐赠表在没有插入硬币时会发出警报

> 原文：<https://hackaday.com/2012/08/15/donation-meter-raises-alarm-when-not-plugged-with-coins/>

![](img/e2fa4f50f471549abaa9baaea8a1f555.png "donation-meter-raises-the-alarm")

这是一种强制性的捐赠计量器。如果你不喂它硬币[，它会持续发出很响的警报](http://blog.devae.re/?attachment_id=29)。

[Piet De Vaere]为比利时根特的一个免费节日制作了这个装置。其目的是帮助提高人们的认识，尽管免门票，但活动的成功取决于捐款。它的工作原理很像停车计时器。当你投币的时候，时间会被加到计时器上。当它一直向下运行时，箱子右侧的大扬声器就会发出警报。

在休息之后的视频中，[Piet]带领我们进行了一次演示，然后参观了硬件。仪表上的指针是一块连接到伺服系统的纸板。Arduino 板控制伺服系统，每当硬币进入滑槽并经过光学传感器时，就会以两分钟的间隔增加时间。硬币的种类没有区别。

使用一个比萨饼盒子作为原型板表明，你不必花心思去建造一些整洁的东西。

[https://www.youtube.com/embed/0bW_mXoJzjo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/0bW_mXoJzjo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)