# 物理橙色通知您 Reddit 消息

> 原文：<https://hackaday.com/2012/10/20/physical-orangered-notifies-you-of-reddit-messages/>

![](img/eafe05898374bdde04c3191c59f08b86.png "Orangered")

任何在 Reddit 上呆过足够长时间以至于激怒 hive mind 的人都很熟悉橙色图标，每当你收到新消息时，你用户名旁边的信封图标就会以美丽的橙色点亮。[Brad]想要一个更显眼的橙色显示器，所以他创建了一个独立的 Reddit 消息指示器,放在他的桌子上，每当有新消息发出时就会亮起。

[Brad]的新橙色通知器的外壳取自廉价旧货店的时钟。在分发完机械机芯后，[Brad]将一个 Arduino、三个 led、一个扬声器以及一个让人想起 Reddit 消息图标的小信封标志装入了漂亮的木箱。

Arduino 连接到运行这个 Perl 脚本的笔记本电脑上。该脚本抓取从 Reddit API 返回的 JSON，如果收到新消息(Arduino 的[源](http://pastebin.com/mwaMdyR3)和 [notes.h 头文件](http://pastebin.com/HTiJ9H2X))，则通过串行端口向 Arduino 发送命令。收到新信息时，Arduino 会点亮信封图标，并在连接的扬声器上播放一小段声音。

[Brad]计划对他的橙色指示器进行一些改进。首先是获得一个以太网屏蔽，并丢弃连接到 Arduino 的服务器。接下来是不同类型消息(PMs、评论回复和 mod 邮件)的不同灯光和音调。当然，我们对[布拉德]未来改进的首要目标实际上是让 led 变成橙色，但这仍然是一个非常棒的构建，允许[布拉德]在互联网的时间接收器上浪费更多的时间。

休息后的视频。

[https://www.youtube.com/embed/Fz43V7B2zMY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Fz43V7B2zMY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)