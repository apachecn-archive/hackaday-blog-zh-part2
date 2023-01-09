# 自主机器人用 IPhone 做大脑

> 原文：<https://hackaday.com/2012/06/09/autonomous-robot-uses-an-iphone-for-its-brain/>

![](img/4a847117323c906a5d2848bdcfd12d73.png "ibot")

去年开学时，[Ryan]需要为他的硕士论文提出一个项目。获得机械学士学位。工程学和做他的软件工程的研究生工作允许[Ryan]为他的论文做一些真正酷的事情；他决定将 iPhone 变成一个具有实时视频流、远程控制和物体探测功能的自主机器人。

[Ryan]去年 10 月开始用一个 Arduino、电机护罩和一个[魔术师机箱](http://www.sparkfun.com/products/10825)建造他的 ArduiPhone。该软件基于一个 [iPhone 网络编程教程](http://www.devx.com/wireless/Article/43551/1954)，它打开一个到桌面 PC 的套接字连接，并将命令转发到 Arduino 串行端口。

[Ryan]的 ArduiPhone 更有趣的功能之一是能够将视频直接从手机传输到 Java 应用程序。代替 FaceTime 的是，[Ryan]通过将来自前置 iPhone 摄像头的图像转换成字节数组来传输视频，通过网络发送，并在 Java 应用程序中解码图像。这是低水平的东西，但视频质量非常好，我们可能会在未来看到更多。

一如既往，休息后的视频。

[https://www.youtube.com/embed/HBwjFh5DH7M?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/HBwjFh5DH7M?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent) [https://www.youtube.com/embed/0aj4B6OG3Xc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/0aj4B6OG3Xc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)