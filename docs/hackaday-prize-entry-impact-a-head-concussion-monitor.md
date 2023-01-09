# Hackaday 奖参赛作品:Impact——头部脑震荡监视器

> 原文：<https://hackaday.com/2015/05/10/hackaday-prize-entry-impact-a-head-concussion-monitor/>

每年都有很多年轻运动员发生脑震荡，却没有被诊断出来，导致脑损伤。[亨特·斯科特]正在研究一种叫做[Impact](https://hackaday.io/project/5613-impact)的设备，以帮助早期检测这些事件。根据[这篇讨论脑震荡识别和评估问题的文章](http://www.momsteam.com/problem-underreporting-concussions-helmet-sensors-solution-to-problem),“在体育运动中早期识别疑似脑震荡是至关重要的，因为在大多数情况下，在遭受脑震荡或其他创伤性脑损伤后立即脱离接触或碰撞运动的运动员会很快康复，不会发生事故。然而，如果允许运动员继续比赛，他们的恢复可能需要更长的时间，他们患长期疾病的风险也更大”

该设备是一个硬币大小的磁盘，它有一个 ATTiny85 微控制器，存储数据的存储器，一个加速度计和一个 LED，当预设的撞击阈值被突破时，LED 就会被激活，所有这些都由一个硬币电池驱动。这种小尺寸使其能够轻松嵌入头盔等运动装备中。在游戏结束时，如果 LED 闪烁，玩家就会被检查是否有脑震荡。为了进行额外的分析，可以下载存储在板载存储器中的数据。这可以通过基于 pogo-pin 的扩展坞来实现，这也是[Hunter Scott]仍在努力的方向。

他有个功能问题需要解决。ATTiny85 不能在安装加速度计的情况下进行编程。他首先需要组装 ATTiny85，对其进行编程，然后组装加速度计。他正在努力解决这个问题，但是如果你有任何建议，请在下面的评论中加入进来。我们想补充的是[ [Hunter](http://hackaday.com/?s=hunter+scott) ]是一个多产的黑客。他的项目[超宽带无线电模块](http://hackaday.com/2014/08/29/thp-entry-level-ultrawideband-radio/)是去年 Hackaday 奖的半决赛项目。

* * *

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)