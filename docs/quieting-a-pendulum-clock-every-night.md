# 每晚让摆钟安静下来

> 原文：<https://hackaday.com/2012/04/01/quieting-a-pendulum-clock-every-night/>

![](img/6367ab078420893ad0069cccf2ae3838.png "clock")

[姚一奇]从他的祖母那里得到了一个很棒的旧钟；这是一件精致的古董，配有真正的机械机芯和一套每小时响一次的迷人铃铛。不幸的是，那些钟声在凌晨 2 点钟有点打扰邻居。以前，[姚一奇]每天晚上都会停止时钟，并希望他能记得在 12 小时后启动钟摆。这是一件苦差事，所以他[决定自动化这个过程](http://www.rurandom.org/justintime/index.php?title=Antique_Clock_Start_Stop_Automation)。

建筑简单而巧妙；一个小的步进电机安装在钟摆下面的钟里。每隔 12 小时，步进电机移动一个杠杆，在十几秒钟的时间内慢慢停止钟摆，让时钟停止运转。12 小时后，马达再次转动，使钟摆开始运动。

这种构建的部件数量非常少——基本上只有一个 ATmega88、一个驱动步进器的达林顿阵列和一个 32.768kHz 的晶体。我们可以想到一些朋友和亲戚家里有很响的钟，所以我们可能要做几个送出去。

休息之后看看演示视频，看看[姚一奇]每晚是如何停止他祖母的时钟的。

[https://www.youtube.com/embed/FZ_Zd7TeMg0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/FZ_Zd7TeMg0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)