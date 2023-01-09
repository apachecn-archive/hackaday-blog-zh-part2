# 将操纵杆与 Xbee 直接连接

> 原文：<https://hackaday.com/2012/05/09/directly-interfacing-a-joystick-with-an-xbee/>

![](img/c02deb9ee600815ce549659fb4a0d54c.png "xbee_joystick_overview")

我们看到使用 Xbee 模块的项目相当稳定。它们是为您的项目添加无线元素的最可靠、最受欢迎的方式之一。但我们并不经常看到他们发挥出全部潜力。由于板上有一个微控制器，许多简单的任务可以完成，而不需要额外的微控制器。[Stephen's]展示了如何通过仅使用 Xbee 模块从游戏控制器读取操纵杆和按钮数据来实现这一点。

他的测试设置使用 Arduino 来驱动硬件接收端的伺服电机。你不能用 Xbee 做所有的事情，但是发送者是这个概念发挥作用的地方。[Stephen]拿了一个旧的游戏手柄，这是一个 PC 游戏端口。操纵杆使用电位计来测量位置数据，按钮只是完成一个电路。他改变了操纵杆,在电位计上增加了分压器，在按钮上增加了上拉电阻。从那里，他只要把它连接到 Xbee 上，[设置模块的固件](http://ilektron-x.blogspot.com/2011/07/xbee-enabled-joystick-part-ii.html)来打包和传输数据。这是一种事半功倍的好方法。

我们在 Hackaday 这里讨论了一下 Xbee 模块，它似乎供不应求。我们中的一些人认为这是由于泰国的洪水。如果你有一些关于这种情况的信息，或者只是想分享你自己的阴谋论，请在评论中告诉我们。