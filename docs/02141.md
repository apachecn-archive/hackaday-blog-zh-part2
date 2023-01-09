# 用相机优化您的电子项目

> 原文：<https://hackaday.com/2012/11/19/optimizing-your-electronics-projects-with-a-camera/>

![](img/19679036c20e3d7396732f26c2b2f2b2.png "LED")

当您有一个要优化的微控制器时，您会怎么做？一种方法是使用调试器，但对于 AVR 等这不是一个非常常见的技术。对于较低层次的电子项目，这几乎是不可能的。[Cnlohr]建立了一个小型《我的世界》服务器，监听游戏中的红石电路，但他的真实世界到街区世界的桥牌性能并不是他所希望的。他想出了一个非常聪明的方法来找出是什么让他的服务器变慢，而不需要任何特殊的设备。

[【cnlohr】的《我的世界》服务器](http://hackaday.com/2012/11/16/avr-minecraft-server-lets-you-toggle-pins-from-the-virtual-world/)只是一个简单的 AVR 微控制器，以太网适配器，和贴在漂亮的玻璃 PCB 上的 SD 卡。他的服务器的性能没有达到他的预期；从服务器下载一个比较大的文件，结果下载速度大概是 55kbps，比他预期的慢很多。他不太确定是什么原因，所以他拿了一部相机，用长时间曝光拍了一张非常模糊的照片。

《我的世界》服务器有一个蓝色 LED 指示灯，用于显示 SD 卡何时被访问。在上图中，[cnlohr]发现 SD 卡访问时间太长，如果他想优化代码，这将是开始的地方。

对于一种非常简单的方法来说，这并不坏，这种方法可以看出微控制器项目中的代码在哪里变慢了。

[https://www.youtube.com/embed/bHbeFnSWSxI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/bHbeFnSWSxI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)