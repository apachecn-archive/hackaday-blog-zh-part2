# 3 美元的无线微控制器/PC 接口

> 原文：<https://hackaday.com/2013/05/19/wireless-microcontrollerpc-interface-for-3/>

![uc](img/631b55363dd16eb98a4ce9fd4b2ff5e5.png)

从微控制器向 PC 发送数据通常需要某种串行连接，要么通过复杂的片上 USB、FTDI 芯片，要么通过昂贵的无线电 IC。[Scott]在创建无线温度传感器网络时不想处理这个问题，[所以他破解了一些便宜的 433 MHz 无线电发射器](http://www.swharden.com/blog/2013-05-19-wireless-microcontroller-pc-interface-for-3-21/)和接收器，以大约 3 美元的价格将数据传输到 PC。

在传感器数据被收集到微控制器上并通过无线电发送出去之后，还有一个问题就是如何把它输入电脑。为此，[Scott]将数据传输到廉价 USB 声卡的麦克风端口。[在微控制器领域和通过盒式接口将程序加载到 Commodore 64 上之前，我们已经见过这个技巧。](http://hackaday.com/2011/07/10/sound-card-microcontrollerpc-communication/)

一旦数据被发送到声卡，它就会被一个小的 Python 应用程序解码。考虑到射频发射器和接收器的范围和质量，[Scott]说这不是一种非常可靠的向 PC 发送数据的方式。虽然它很便宜，但是如果你需要在预算内无线读取传感器，很难做得更好。

看看下面[斯科特]的创作演示。

[https://www.youtube.com/embed/GJHFldPwZvM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/GJHFldPwZvM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)