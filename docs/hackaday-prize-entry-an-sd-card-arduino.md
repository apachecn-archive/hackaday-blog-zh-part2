# Hackaday 奖品入口:一张 SD 卡 Arduino

> 原文：<https://hackaday.com/2015/06/28/hackaday-prize-entry-an-sd-card-arduino/>

大约一年前，英特尔宣布他们将推出一个嵌入 SD 卡的新平台。想象一下——一台完整的计算机被封装到一个 SD 卡中，有九个完整的引脚用于电源和 I/O。为什么不能在 SD 卡里装一个 Arduino？

[kodera2t]发现没有真正的理由为什么你不能把一个小的微控制器放在 SD 卡里。为了他的 Hackaday 奖参赛作品，[他创造了 SDuino](https://hackaday.io/project/6435-sd-card-sized-board-lets-say-sduino) ，它就像罐头上写的那样:一个 ATMega328p 被塞进一个 microSD 适配器。

与 SD 卡平台中的另一个微控制器不同，在大多数情况下，[kodera]尊重 SD 卡的标准引脚排列。当然，MISO 和 MOSI 信号是相反的，SD 引脚上的一个地连接到微控制器上的一个模拟输入引脚，SD 引脚上的片选完全被忽略。除此之外，它是最接近带微控制器的 SD 卡。

* * *

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)