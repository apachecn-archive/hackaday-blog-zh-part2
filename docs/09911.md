# Hackaday 奖半决赛选手:CANcrusher

> 原文：<https://hackaday.com/2015/08/25/hackaday-prize-semifinalist-cancrusher/>

2007 年，所有人都发现你可以用 Arduino 让 LED 闪烁。几年后，有人发现你可以用 Arduino 让 PID 控制器工作，于是互联网上出现了大量的 sous vide cooker 黑客。电子项目的趋势来来去去，今年我们有了 CANbus 嗅探器和开发平台。其中一个 CAN dev 平台 [CANcrusher](https://hackaday.io/project/7181-cancrusher-car-hack-development-platform) 是 Hackaday 奖的半决赛选手，在戳戳 CANbus 方面做得很好。

像许多非常优秀的项目一样，CANcrusher 基于一个 Teensy 3.1 微控制器。它与 MCP2515 CAN 控制器一起为 CANcrusher 提供了三个独立的 CAN 通道，支持 DW-CAN、SW-CAN 和 LSFT。该设备的软件可以通过 USB 将数据直接传输到电脑。

简单地为 CAN 总线提供一个接口是一件已经做得很死的事情，为了改进现有的许多 CAN 总线项目，CANcrusher 增加了蓝牙、GSM 无线电、SD 数据记录和实时时钟。这是 Hackaday 奖的一个伟大项目，有多个视频解释它是如何工作的，它能做什么。你可以看看下面的参赛视频。

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)

[https://www.youtube.com/embed/UfGwF-g6ROA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/UfGwF-g6ROA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)