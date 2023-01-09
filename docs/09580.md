# 与(机器人)手交谈

> 原文：<https://hackaday.com/2015/07/19/talk-to-the-robotic-hand/>

机器人黑客[Andrea Trufini]显然喜欢选择。他的机械臂不仅有六个自由度，而且有多种方式可以控制它。该手臂的软件可以通过编程语言、电位计、红外遥控器或者——真正有趣的部分——通过口头命令接受命令。

视频没有显示太多的构建细节，但手臂主要由激光切割胶合板构成，并使用 Arduino。希望我们能很快看到更多关于这个版本的细节，但是现在先看看类似的项目。

该软件(myrobotlab)在 [github](https://github.com/MyRobotLab/myrobotlab) 上，看起来非常令人印象深刻。基于 Java 的框架有一个面向服务的架构，模块支持常见的处理器(如 Arduino、Raspberry Pi 和 Beagle Board)以及 I/O 设备(如电机、声音设备和您必须购买的 Leap Motion 控制器)。从下面的演示中，你可能会想到，还有语音到文本和文本到语音的服务。像许多开源项目一样，这些服务中的一些比其他服务更[为黄金时间做好准备](http://myrobotlab.org/download)，但这仅仅意味着你可以将你的黑客技术贡献给项目。

[https://www.youtube.com/embed/3wqz29GgQfM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/3wqz29GgQfM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

你可以用这样的框架建造一些非常强大的机器人。有多厉害？其中一个服务知道如何下国际象棋。