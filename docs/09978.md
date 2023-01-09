# 低于 50 美元的 2 线 Arduino 视频:台面视频

> 原文：<https://hackaday.com/2015/09/01/arduino-video-over-2-wires-for-under-50-mesa-video/>

如果你想在你的项目上获得视频支持，你可以从一个内置的设备开始，比如树莓 Pi。[Kevinhub88]不接受这样的妥协，所以他和他的 Black Mesa 实验室想出了一种全新的方法，为 Arduino 和其他廉价控制器等设备添加视频支持。这个项目被称为 [Mesa-Video](https://blackmesalabs.wordpress.com/2015/08/30/mesa-video-800x600-digital-video-for-arduinos-over-2-wire-serial-mesa-bus/) ，它可以将分辨率高达 800×600 像素的数字视频添加到任何具有单个串行输出的设备上。

这个视频是由 FTDI 的一个低成本 GPU[ft 813](http://www.ftdichip.com/Products/ICs/FT81X.html)制作的，它通过一个便宜的低功耗芯片~~(他已经演示了用柠檬电池运行)~~提供了惊人的视频效果，这意味着他希望能够以低于 50 美元的价格出售 Mesa-Video。

*更新:[KevinHub88]让我们知道他实际上并没有用柠檬电池给设备供电，因为你需要很多柠檬才能在 5V 下产生 50mA 的电流。对于任何困惑，我深表歉意！*

然而，Mesa-Video 只是一个开始。[Kevinhub88]想要解决 Arduinos 上叠加盾牌的问题:多加一个就麻烦了。他想创建一个更简单、更快速、更开放的接口，所以他创建了 Mesa-Bus。这有效地通过简单、快速的串行连接将 SPI 和 I2C 流量包装在一起，不需要太多解码。这意味着你可以通过几根电线发送电力和双向数据，同时还可以连接多个设备，并根据需要进行交换。例如，您可以在 PC 上进行开发工作，通过 Mesa-Bus 与原型设备进行对话，当您的第一个版本在您的开发环境中运行时，可以将 PC 换成 Arduino。Arduino 没有切吗？因为 Mesa-Bus 是跨平台和开源的，所以很容易将 Arduino 替换为 Raspberry Pi，而无需更改其他设备。而且，因为所有数据都通过简单的串行连接以纯文本的形式传输，所以很容易调试。

这是一个雄心勃勃的项目，而且[Kevinhub88]还有一段路要走:他目前正致力于让他的第一个原型 Mesa-Bus 设备启动并运行，并最终完成 Mesa-Video 的设计。但这是一个令人印象深刻的开始，我们将密切关注这项工作。希望他也能避免头蟹的问题，因为那些东西非常痒。