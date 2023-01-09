# Hackaday 奖参赛作品:通过 WiFi 控制继电器

> 原文：<https://hackaday.com/2015/07/04/hackaday-prize-entry-controlling-relays-over-wifi/>

距离 ESP8266 WiFi 模块发布还不到一年。这款芯片的原始数据表只有中文，只能通过 AT 命令控制，并且(最初)只通过 Seeed Studio 和其他各种中国零售商销售。它有一个优点:它是五美元。为了一个蹩脚的潜艇的价格，你可以从互联网上眨一下 LED。不用说，ESP8266 现在非常受欢迎。

今年的 Hackaday 奖有很多 ESP8266 项目，[【David】的项目](https://hackaday.io/project/6456-esp8266-din-8-channel-wifi-relay-controller)很大程度上利用了这个模块相对微薄的引脚排列。他建造了一个 8 通道继电器控制器，带有 WiFi 接口来控制工业设备。这是一个伟大的项目，但只是今年获奖的许多 ESP 项目中的一个。

ESP 没有太多的引脚，但是如果有合适的硬件，对于一些严肃的工作来说已经足够了。他使用 ESP-12 模块来获得最多的引脚，并使用 SPI 端口扩展器来驱动一组继电器。这是一个简单的板，但你需要通过 WiFi 控制一堆继电器的一切都在那里:led，复位按钮和 RS232 电平转换。

你可以看看下面一对非常令人满意的接力点击视频。

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)

[https://www.youtube.com/embed/bYWmRU5XIWA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/bYWmRU5XIWA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/y9DlE2H5v3U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/y9DlE2H5v3U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)