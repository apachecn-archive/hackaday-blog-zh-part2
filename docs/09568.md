# 用树莓派追踪几乎每架飞机

> 原文：<https://hackaday.com/2015/07/18/tracking-nearly-every-aircraft-with-a-raspberry-pi/>

FlightAware 是实时追踪世界各地飞机的首要网站，在过去一年左右的时间里，Raspberry Pi 的所有者一直在通过检测头顶上飞行的飞机并将数据发送到 FlightAware 服务器来为 FlightAware 网络做出贡献。

到目前为止，这些志愿者一直使用 Raspis 和软件定义的无线电模块来监听从飞机上传输的 ADS-B 消息。随着 FlightAware 对 PiAware 的新更新，他们的 Raspberry Pi 航班跟踪软件、 [Mode S 转发器也可以被检测到并添加到 FlightAware 网络](https://discussions.flightaware.com/ads-b-flight-tracking-f21/multilateration-mlat-now-available-on-piaware-t35637.html)。

去年，FlightAware 宣布，任何拥有 Raspberry Pi(一个软件定义的无线电模块)和互联网连接的人[都将获得一个免费的 FlightAware 企业账户](http://hackaday.com/2014/08/25/piaware-automated-airliner-tracking-on-the-raspberry-pi/)，用于收听头顶飞过的 ADS-B 发射器，并将信息发送到 FlightAware 服务器。ADS-B 对飞行员来说是一个相对较新的要求，它将飞机的标识、GPS 坐标、高度和速度传输给控制人员和其他任何想知道谁在头顶上飞行的人。

另一方面，S 模式转发器是较老的技术，只是简单地发送飞机的呼号。没有传送 GPS 信息或高度信息，但通过新版本中一些巧妙的多边定位，这些转发器和飞机现在可以被跟踪。

为了获得这些转发器的位置，至少三个其它的便携式盒子必须接收来自 S 模式转发器的信号。这些信号，连同它们被接收时的时间戳，然后被发送到 FlightAware 服务器，在那里可以确定应答器的位置。

此次更新的最终结果是，FlightAware 现在可以跟踪全球两倍多的飞机，所有这些都只需简单的软件更新。这是众包软件定义无线电模块最成功的应用之一，如果你想参与其中，FlightAware 团队整合了一个批量订购的 ADS-B 天线。