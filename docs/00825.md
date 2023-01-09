# 使用 Raspi 作为以太网屏蔽

> 原文：<https://hackaday.com/2012/06/24/using-the-raspi-as-an-ethernet-shield/>

![](img/cd93bee9fb3e9cce282e36c06ea1dab1.png "ardupi")

[Alexandre]想用他的 Arduino 设置一个基于网络的温度记录器，但发现 Arduino 以太网屏蔽有点挑剔。由于他的 Raspberry pi 刚刚发布，他认为只需一点点编码就可以将 Raspi 用作以太网屏障。

在[Alexandre]设置他的 Arduino 通过 USB 发送热电偶后，剩下唯一要做的就是将 [node.js](http://nodejs.org/) 添加到 Raspi 的 Debian 安装中。每隔五分钟，Arduino 就会醒来，读取温度读数，并将其发送到树莓 pi。从那里，很容易解析 Arduino 的 JSON 输出，并在 web 上提供。

最终，[Alexandre]成功地将他的 Raspberry pi 设置成了一个以太网屏蔽，为[一个显示当前温度的网页提供服务](http://pc.alapetite.fr:8080/temperature)(顺便说一下，不要 F5 那个链接)。我们必须指出的一件有趣的事情是设置这个在线温度记录器的成本:Arduino 以太网屏蔽[售价 45 美元](http://www.sparkfun.com/products/9026)，而树莓 pi 售价 35 美元。是的，使用树莓 pi 作为以太网屏蔽实际上比目前的 Arduino 产品*更便宜*。给你吧，以防万一你对拉斯皮的事还犹豫不决。