# 透明闹钟运行 Linux

> 原文：<https://hackaday.com/2015/05/30/transparent-alarm-clock-runs-linux/>

[Benoit]用的是一个非常旧的闹钟，通常靠市电供电，他把它插在电脑的 UPS 上，让它在停电时也能工作。他注意到，当 UPS 打开时，时钟会跑得很快，显然它是通过观察电力系统频率来计时的。为了解决这个问题，他创造了自己的[功能密集型时钟，运行 Linux](http://www.bfrigon.com/posts/projects/alarm-clock/) 。

这款闹钟拥有一切:透明环氧树脂封装的七段显示器，触摸界面，电池备份，从 [NTP](http://en.m.wikipedia.org/wiki/Network_Time_Protocol) 服务器检索时间的能力，以及通过网络改变时钟设置的网络界面。这是[Benoit]决定让时钟运行 Linux 的主要原因；网络功能为时钟增加了许多功能，例如在特定时间向其他设备发送命令的功能。时钟运行在一个 Aria G25 SOM 上，并有一个定制的外壳，看起来非常专业。

我们喜欢这里的高质量时钟，而[Benoit]最近的项目击中了我们所有的按钮。尽管目前还没有[让人发疯](http://hackaday.com/2011/10/06/vetinari-clock-will-drive-you-insane/)或[告诉令人困惑的时间](http://hackaday.com/2014/09/22/topsy-turvy-clock-tells-confusing-time/)，Linux 和网络功能肯定会打开选择的大门！