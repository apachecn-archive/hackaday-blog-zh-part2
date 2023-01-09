# 韦小宝用射频在房子里追踪你

> 原文：<https://hackaday.com/2015/01/24/trinket-uses-rf-to-track-you-through-the-house/>

如果你带着带 GPS 的手机，你总是知道你在地球上的什么地方。但是在建筑物内部或者甚至你自己的家里呢？知道你是在厨房还是客厅将是家庭自动化系统的一大特色。当你进入房间时，灯会亮着，你的音乐会随着你进入家庭音响系统。这正是[Eric]正在利用一个袖珍收发器项目进行的无线电定位工作。[Eric]开始这个项目是为了参加日常携带小饰品比赛。他没有进入前 3 名，但却是让比赛变得非常难以评判的激烈竞争者之一！

该项目的核心是确定无线电信号的飞行时间。由于无线电波以光速移动，这对于基于 Arduino 的设计来说是一个不小的壮举！[Eric]并没有重新发明轮子——他的设计基于几篇研究论文，他把这些论文与他的项目描述联系起来[。当计算往返时间而不是单程时间时，飞行时间的计算变得更容易处理。为了处理这种情况，一个或多个基站发出 pings，由用户佩戴的小型转发器接收并返回。通过对多次往返传输进行平均，可以计算距离估计。](http://hackaday.io/project/3464)

[Eric]使用了一个 Pro Trinket 作为他的移动转发器，而一个 Arduino Micro 及其 16 位计数器作为基站。对于射频，他使用了流行的北欧 nRF24L01+ 2.4 GHz 收发模块。即使是这样简单的硬件，他也取得了巨大的成就。到目前为止，他可以在图表上显示基站和转发器之间的距离。不坏的 DIY 转发器这么小，如果适合在一个 2xAAA 电池盒！[Eric]下一个任务是解决多路径问题，并测试多个基站。

点击休息时间观看[Eric 的]项目！

[https://www.youtube.com/embed/1elSnGPEPEc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/1elSnGPEPEc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)