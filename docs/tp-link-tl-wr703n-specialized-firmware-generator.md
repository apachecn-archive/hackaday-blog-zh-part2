# TP-Link TL-WR703N 专用固件生成器

> 原文：<https://hackaday.com/2013/01/18/tp-link-tl-wr703n-specialized-firmware-generator/>

在这个图像的中心看到的是一个 TP-Link TL-MR3020，它基本上是一个带有几个额外 led 的 TL-WR703N 无线路由器。我们已经看到很多项目使用这种硬件，因为它便宜，适合黑客攻击。这些设备可以运行 OpenWRT，这是一个用于路由器的 Linux 发行版，与普通固件相比，它极大地扩展了功能。现在，Shackspace——一家位于德国斯图加特的黑客空间——的几个成员已经编写了一个脚本，可以自动为路由器生成专门的固件。那个链接指向他们关于剧本的维基页面，但是你可能会发现[这篇概述文章](http://shackspace.de/?p=3772)更容易阅读。

这个概念是，将专门的黑客收集到易于闪存的包中，可以消除许多令人头疼的配置问题。例如，如果您只想在一整天的活动中使用 NFC 读卡器，您可以像上面看到的那样连接硬件，并使用脚本的 NFC-gate 选项来刷新驱动它的固件。到目前为止，还支持流 USB 摄像头，作为 USB 网桥，以及其他一些功能。但这样做的全部目的是使将新的固件模块加入脚本变得简单，从而便于保存工作以备后用。

[谢谢哈迪斯]