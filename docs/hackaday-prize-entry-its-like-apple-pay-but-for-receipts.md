# Hackaday 奖参赛作品:它类似于 Apple Pay，但用于收据

> 原文：<https://hackaday.com/2015/07/06/hackaday-prize-entry-its-like-apple-pay-but-for-receipts/>

有 Apple Pay，Samsung Pay，Google Wallet，以及许多其他用手机支付的方式。但是收据呢？你真的需要随身携带小纸片向怀疑的朋友证明你确实买了一个甜甜圈吗？证据在家里的档案里。在 D 下面，代表甜甜圈。

[Hisham]正在为 Hackaday 奖开发一个非常有趣的系统。这实际上是 Apple Pay、Samsung Pay 和 Google Wallet 正在进行的每一项销售点交易的对立面。[【his ham】的 Aelph 不处理付款，而是处理收据](https://hackaday.io/project/4665-aleph)。

[Hisham]的项目是硬件，带有一个插入销售点终端的小型设备。该设备将收据传输到 Aleph 应用程序(或第三方应用程序)，并将收据的 PDF 副本上传到服务器。除了一个小硬件盒，POS 终端不需要额外的软件。对于零售商来说，就像插上盒子一样简单，对于消费者来说，就像下载一个 app 一样简单。

硬件原型在 TI LaunchPad 上实现，配备 TIVA C 微控制器。这与 NFC 评估套件一起给了 Aleph 足够的能力来连接到公司局域网并生成一些 pdf 文件。你可以看看下面[Hisham]的一个演示视频。

电子收据有很多好处；如果你需要一张收据，无论如何你都会扫描它的*—*一张枯树收据效率很低。热敏收据纸里也有一些有害的化学物质。你只需要谷歌一下 BPA 收据就能找到证据。无论哪种方式，这都是一个好主意，我们渴望有一天我们的钱包不会被塞得像克斯坦萨式的比例，我们不需要扫描仪来完成支出报告。

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)

[https://www.youtube.com/embed/4xHYaepuHeU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=26&wmode=transparent](https://www.youtube.com/embed/4xHYaepuHeU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=26&wmode=transparent)