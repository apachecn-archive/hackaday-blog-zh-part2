# 打破古怪的光轮

> 原文：<https://hackaday.com/2014/05/17/breaking-open-the-quirky-nimbus/>

![Nimbus](img/3e6e74a1ca2ecca27ebe137e599c8d94.png)

Nimbus 是一家名为 Quirky 的公司推出的一款联网设备。它有四个模拟表盘，每个都有图形液晶显示器，有 WiFi 连接，可以显示你在过去一天发了多少条推文。你知道，万一你忘了，或者什么的。

[Edu]不觉得面向社交媒体的光轮非常有用，但互联网连接的模拟仪表只是*太酷了*，所以[拿出了螺丝刀，开始编写新固件](http://blog.arcnor.com/2014/05/15/quirky-nimbus-hacking/)。

在 Nimbus 内部有一个 SPI 闪光灯、PIC micro 和一个电动 Imp，一个微型 ARM 微控制器和一个装在 SD 卡内的 WiFi 适配器。Imp 总是与云服务联系在一起，在这种情况下，是一种古怪的云，但古怪的人热衷于帮助[Edu]寻求更好的固件。

在弄清楚所有的痕迹后，[Edu]编写了一个简单的固件，可以控制所有要控制的东西——刻度盘、显示器、两个按钮和一个扬声器。到目前为止，他已经在显示器上放了一些图片，并对《猴岛》的主题进行了脉宽调制。这只是该设备所能做的表面工作-[ edu]仍然可以利用 WiFi 连接，这些拨号盘可以做的远不止转圈。

下面猴岛视频。

[https://www.youtube.com/embed/R2kULmfCv38?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/R2kULmfCv38?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)