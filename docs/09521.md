# 黑客日奖参赛作品:一个非常小的电网

> 原文：<https://hackaday.com/2015/07/11/hackaday-prize-entry-a-very-small-power-grid/>

如果你现在还不明白，电网是令人惊讶的技术奇迹，很可能是历史上最伟大的工程壮举之一。学习这些系统如何工作在理论上很容易，但在实践中，如果你试图在发电站乱搞，你会被击中。[Tim]和[Marissa]认为一定有更简单的方法来了解电网[，所以他们制作了自己的](https://hackaday.io/project/6290-smart-grid-test-facility)。它很小，但是它仍然拥有你在高压电线中能找到的一切，大约负 100 千伏。

这个电网模型通过将一个普通的 DC 发动机连接到交流发电机和变压器来模拟发电厂。这是两个模拟发电点，第三个 AC/AC 电源用作同步相位和频率的参考发电机。60Hz 时只有 12V，但它能完成任务。

电网不是发电厂，还有传输线理论。为此，[Tim]和[Marissa]准备了几块装有电感的电路板来模拟电力线。MSP430 上有模拟负载板和同步系统。

在下面的视频中，[Marissa]查看了系统的所有进出信息。它制作得非常好，非常适合教授没有实际例子就无法演示的东西。

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)

[https://www.youtube.com/embed/rrS2u2TGiJs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/rrS2u2TGiJs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)