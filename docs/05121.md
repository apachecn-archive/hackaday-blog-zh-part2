# 给我倒杯酒，德林克莫。

> 原文：<https://hackaday.com/2014/01/21/make-me-a-drink-drinkmo/>

【Cabe Atwell 的】最新项目是一件艺术品，让我们来介绍一下 Drinkmotizer: [一个树莓 Pi 饮品搅拌机器人。](http://www.element14.com/community/community/raspberry-pi/raspberrypi_projects/blog/2014/01/17/raspberry-pi-drink-mixing-robot--aka-the-drinkmotizer)

正如[Cabe]所说，几乎每个工程师的待办事项清单上都有一个调酒机器人。我们可能不得不同意。它们很实用，很酷，在聚会上很有用。

> 在你的聚会上，你需要调酒器…在某些时候，在聚会上，调酒的技巧丧失了。
> 
> 德林克莫是你指定的清醒的调酒师。
> 
> 你的推动者。
> 
> 你的朋友。

Drinkmo 的工作原理是旋转一根长丝杠，将混合杯从一个瓶子移动到另一个瓶子。整个装置由铝挤压制成，本质上是完全可扩展的。在最上面的架子上是由 12v 直流汽车锁致动器控制的重力供给子弹分配器。追逐者站(在尽头，右边)的工作方式不同。追逐瓶实际上是由彩弹枪罐加压，并使用电磁阀分配。考虑到彩弹罐的压力范围可以从 1000-3000 磅/平方英寸，我们希望他有一个压力调节器。

整个系统由运行 Raspbian 的 Raspberry Pi 控制，[Cabe]使用 Tkinter 作为程序的 GUI。他在上面链接的原始论坛帖子上有大量信息(包括示意图！)，如果你在休息后留下来，有一个制作非常好的 Drinkmo 视频。

[https://www.youtube.com/embed/B87Y0zwaywI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/B87Y0zwaywI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)