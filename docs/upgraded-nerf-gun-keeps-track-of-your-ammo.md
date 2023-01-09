# 升级的 Nerf 枪可以追踪你的弹药

> 原文：<https://hackaday.com/2014/07/09/upgraded-nerf-gun-keeps-track-of-your-ammo/>

[Paul]和他的伙伴[Jonathan]最近参加了一个僵尸主题的 Larp 活动，所以本着让体验更真实的精神，他们决定[升级他们的 Nerf N-Strike Stryfe 枪](http://imgur.com/a/vOcmn)。

他们首先打开枪，记下一些铃铛和哨子的可用空间。幸运的是，由于传统的塑料注射成型实践，有很大的空间！

升级包括一个弹匣传感器，一个堵塞传感器，一个触发传感器和一个电压表，使枪变得更加智能。山寨版 Arduino Pro Mini 接收所有这些输入，并将其输出到 7 段 LED 显示屏，以便于查看。我们最喜欢的部分是弹药传感器，它可以记录你用了多少发子弹。它只是一个达林顿配置的红外光电二极管和红外晶体管，连接到假 Arduino 上的 GPIO 中断引脚。

[https://www.youtube.com/embed/X6Rc4qa31F0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/X6Rc4qa31F0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

这不是一个过于复杂的项目，但执行得非常好——也许 Nerf 应该在未来采用这样的东西！仍然在等待[一个自动哨兵炮塔虽然……](http://hackaday.com/2013/07/03/sentrifying-a-nerf-gun/)

如果你对僵尸王感到好奇，你可以在这里找到它的一切！