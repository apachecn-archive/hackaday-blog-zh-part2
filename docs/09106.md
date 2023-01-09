# Hackaday 奖参赛作品:生物电位信号库

> 原文：<https://hackaday.com/2015/05/22/hackaday-prize-entry-biopotential-signal-library/>

随着今年 Hackaday 奖的修复术、脑电图和所有其他专注于身体和医学的构建，看看测量来自人体的微小电信号需要什么可能是一个好主意。在室内测量脑电波或心跳很难；对于这些测量，交流电源频率很容易耦合到高阻抗输入，信号本身非常非常弱。为了获得 Hackaday 奖，【Paul stoff regen】[正在开发工具，使 EEG、ECG 和 EMG 的测量变得简单，只需使用廉价的工具](https://hackaday.io/project/5809-biopotential-signal-library)。

如果这个名字听起来很熟悉，那是因为他是微控制器板家族和几十个非常受欢迎的库的幕后人物，这些库包括从显示器到实时时钟的所有东西。生物电位信号库延续了[Paul]的传统，只用代码就能构建非常酷的东西。

本项目使用的硬件是 TI 的 ADS1294，一款 24 位 ADC，具有 4 或 8 个通道。这款芯片作为*医疗*模拟前端投入市场，为了更好地测量，还加入了一点心电图。[Paul]最初只使用 ADS1294 以后可以添加更多的模拟芯片。这本身就是一个伟大的项目，当你包括这个库的潜在应用时——从假肢到身体传感器的一切——它将成为一个令人敬畏的 Hackaday 奖条目。

* * *

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)