# Hackaday 奖品入口:当你不能时，NetBOOT 使你的调制解调器循环

> 原文：<https://hackaday.com/2015/08/22/hackaday-prize-entry-netboot-powercycles-your-modem-when-you-cant/>

许多人将家庭网络设置为动态 dns 服务，以便远程访问他们的文件、打印机或基于 Pi 的安全摄像头系统。许多人也遭受不太好的互联网连接，并发现自己无法访问他们的家庭系统由于停滞的信号。

netBOOT 是一个基于 Arduino 的设备[，当你无法重置调制解调器时，它会自动为你重置调制解调器](https://hackaday.io/project/7288-netboot)。该系统的核心是一个标准的基于 ATMEGA328p 的 Arduino 板，结合一个 W5100 以太网模块和一个继电器模块。Arduino 上的软件定期 pings 一系列 IP 地址并监听响应。如果在 3 次尝试中没有找到，与调制解调器的 DC 电源串联的继电器模块将被打开 10 秒钟，然后返回关闭状态。一旦你的调制解调器重新启动并重新同步，一切都应该准备就绪。

我们不记得在谷歌新 OnHub 的规格列表中看到过这个功能。重置不良连接的能力似乎应该成为未来路由器的一项功能，对吗？

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)