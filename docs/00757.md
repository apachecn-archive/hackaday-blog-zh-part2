# 用一个路由器把几十个 Arduinos 放到互联网上

> 原文：<https://hackaday.com/2012/06/18/putting-scores-of-arduinos-on-the-internet-with-one-router/>

![](img/184c95245651a3cabba9864afd2e1d5c.png "jeenode")

像最近的许多黑客一样，[Rick]一直在尝试用废弃的 WiFi 路由器和 OpenWRT 安装将 Arduinos 连接到互联网。与他的同行不同，[Rick]认为将一个路由器专用于一个 Arduino 项目是浪费，所以他使用一个小型、低功耗的无线模块将多达 30 个 Arduino 连接到互联网。

就像最近的几个版本( [1](http://hackaday.com/2012/06/10/using-a-router-as-a-wireless-embedded-platform/) ， [2](http://hackaday.com/2011/08/01/fonera-based-quadcopter-can-be-controlled-from-a-web-browser/) )一样，【瑞克】在他当地的黑客空间发现了一台旧的 Fonera 路由器。安装 OpenWRT 后，[Rick]将一个[非常小的无线模块](http://jeelabs.net/projects/hardware/wiki/JeeNode_Micro)连接到路由器的 GPIO 引脚，并修补固件，在路由器上放置 SPI 总线。

现在，每当[Rick]想要将 Arduino 项目连接到互联网时，他所需要的就是一个 [$4 的无线电模块](http://www.hoperf.com/pro/rf/cob/rfm12b.htm)。这个无线电模块连接到路由器，路由器处理多达 30 个 DIY 项目的网络需求。

如果你想建立一个支持互联网的传感器网络，老实说，我们想不出更好或更便宜的方法。干得好，[瑞克]。