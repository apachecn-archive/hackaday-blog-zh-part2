# Hackaday 奖参赛作品:尽情跳舞

> 原文：<https://hackaday.com/2015/06/26/hackaday-prize-entry-lose-yourself-to-dance/>

不是每个 Hackaday 奖的项目都需要解决一个紧迫的问题，拯救地球，或者帮助人们。有时候，只是需要酷一点。[杰里米]的项目当然很酷。他正在为*周六夜狂热*的魅力和*比利·简*音乐视频的技术复杂性建造一个触摸感应迪斯科地板。

这些年来，我们看到了一些迪斯科舞厅的地板，在大多数情况下，[杰里米]并没有偏离一条良好的道路太远。他使用 LED 灯条来照亮他的建筑，用胶合板和半透明的正方形来切割地板框架，并使用 ATMega 来控制每个面板。目前为止，没什么异常。

这个建筑的诀窍是每个正方形都有一个电容式触摸传感器。每个半透明面板下面都有一点金属丝网。因为迪斯科舞厅有 144 个节点，运行标准的电容传感器库是行不通的；测量每个节点的延迟增加得非常快。通过[重写【Paul Stoffregen】的电容传感器库](https://hackaday.io/project/4209-interactive-disco-dance-floor/log/19764-non-blocking-capacitive-sensing),【Jeremy】能够同时运行许多面板。

现在[杰里米]有一个单一的面板，它对赤脚的反应和对摩托车靴子的反应一样好。这正是你在互动舞池中所需要的，我们迫不及待地想看到整个舞池运行起来。

* * *

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)