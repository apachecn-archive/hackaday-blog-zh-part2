# Hackaday 奖半决赛选手:更好的智能插头

> 原文：<https://hackaday.com/2015/08/29/hackaday-prize-semifinalist-a-better-smart-plug/>

走进任何一家家装商店，你都会发现几十种智能配件、家庭自动化设备和 WiFi 连接的蜉蝣。Belkin WeMo Insight 就是这些设备中的一种，它让任何拥有 60 美元和 WiFi 网络的人都能够通过网络开关灯和电器。[John]拿起了其中一个 WiFi 插头，但它并不完全像他希望的那样工作。[John] [没有从头开始构建智能插头，而是为他的 Hackaday Prize 参赛作品](https://hackaday.io/project/6799-smartee-the-smart-plug)更换了 WeMo Insight 的控制板，使其更加有用，并成为 Kill-a-Watt 等设备的替代品。

在股票形式下，WeMo 只能通过 Belkin 提供的智能手机应用程序或 IFFT 等第三方服务使用。所有这些解决方案都具有有限的 API，并且不提供高级功率指标。为了解决这个问题，[John]用他们自己的设计替换了 Belkin WeMo 内部的智能控制板。

就体积而言，WeMo 内部的大多数电子设备是变压器、电容和继电器；这个智能插头的智能只是一个子板。通过使用新的微控制器、ESP8266 和 microSD 卡连接器重新设计该子板，[John]可以复制 WeMo 的功能，同时添加一些新功能。SD 卡数据记录现在可以长达四年，RTC 现在可以提供所有收集数据的精确时间戳，微控制器上的一些简单计算可以实现功率因数、线路频率和总电能计量。有了 ESP，所有这些数据都可以通过一个大大改进的 API 发送到云中。

这是一个伟大的项目，Belkin 应该在 WeMo 的下一个版本中认真考虑。对于任何一个坚持使用股票 WeMo 的人，[John]已经公开了他所有的设计文件和代码，允许任何人复制这个版本

你可以看看下面[John]的 Hackaday Prize 参赛视频。

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)

[https://www.youtube.com/embed/dbmhl7EVD_Q?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/dbmhl7EVD_Q?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)