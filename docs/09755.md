# Hackaday 奖参赛作品:瓦斯手榴弹帮助，而不是爆炸

> 原文：<https://hackaday.com/2015/08/08/hackaday-prize-entry-gas-grenade-helps-instead-of-exploding/>

如果有人扔了一颗手榴弹，那就有理由认为会有不愉快的事情发生。防暴警察经常使用催泪弹来驱散难以控制的人群，军方可能会使用烟雾弹作为掩护，向武装阵地推进，或标记需要空袭的位置。但是一些气体手榴弹是为了帮助，而不是伤害，就像[这个会说话的气体感应手榴弹](https://hackaday.io/project/4742-gas-sensor-for-emergency-workers)这是 2015 年 Hackaday 奖的参赛作品。

进入受限空间是救援工作中特别危险的一个方面，尤其是在采矿业中。塌方或其他事故不仅会困住人，还会困住危险气体，危及受害者和救援人员。已经开发出了许多新奇的机器人，它们可以在救援人员之前将气体传感器带到密闭空间的深处，但[埃里克·威廉]想出了一种更便宜的方法，在进入之前嗅嗅空气。一个 MQ2 组合一氧化碳、液化石油气和烟雾传感器与一个 Arduino Nano 接口，一个 433MHz 发射机连接到一个输出端。一小段代码测量来自传感器的数据，并合成人的声音读数，然后输入发射机。整个包装被塞进一个结实的、容易展开的包装中——一个 Nerf 狗玩具！扔进一个密闭的空间，手榴弹开始用英语口语大声读出读数，范围内的任何超高频对讲机都能接收到。[Eric]在休息后的视频中报告说，他在一个街区外收到了信号——对于潜在的爆炸性情况来说，这是一个很好的距离。

随着廉价传感器供应的不断增加，像这样的想法有无限的可能性。给手榴弹增加温度、湿度和压力传感器并不难，甚至可以从[这个传感器套件](http://hackaday.com/2013/01/31/gas-sensor-suite-built-with-gadgeteer-modules)中增加酒精和氨传感器。加上像微粒、振动和辐射这样的传感器，很快你就有了一个可以做很多好事的手榴弹。

[https://www.youtube.com/embed/_83s2re38ZU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/_83s2re38ZU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)