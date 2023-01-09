# 在电脑上使用 Boxee 遥控器

> 原文：<https://hackaday.com/2014/10/01/using-the-boxee-remote-with-a-pc/>

当 Boxee 遥控器在 2010 年首次发布时，它是一个天才之举。不是因为它控制了机顶盒，也就是媒体中心的电脑。这给人留下了深刻的印象，因为遥控器的背面有一个小 qwerty 键盘，正好可以用来搜索加载了电影和电视节目的菜单以及输入 URL。[马丁]的 BoxeeBox 喜欢他的 BoxeeBox，但它现在是一个旧设备，对网络流媒体的一些支持(包括网飞)已经消失了。

其他媒体中心设备填补了[马丁]生活中的空白，但他喜欢 Boxee 遥控器。让它在 XBMC 的个人电脑上运行是头等大事。这意味着要想办法将射频接收器从机顶盒连接到 USB 端口。[事实证明这非常简单](http://martinvsamuelsson.blogspot.se/2014/09/boxeebox-remote-on-xbmc.html)，只需要几个零件和半根 USB 线。

[Martin]找到了 BoxeeBox 的 RF 接收器上的连接器，并找到了 USB 电缆中常见的 V+、V-、电源和接地连接。接收器工作在 3.3 伏，所以降压需要稳压器。项目的其余部分只是简单地把所有东西放进项目箱，然后塞到他的电脑后面。

Windows 将 RF 接收器识别为普通键盘，因此一切顺利。自从[马丁]制造了这个小设备，一些人[已经为 XBMC](http://wiki.xbmc.org/index.php?title=Boxee_remote)和 Boxee 遥控器提出了更好的键盘布局，让这个设备在未来也能工作。