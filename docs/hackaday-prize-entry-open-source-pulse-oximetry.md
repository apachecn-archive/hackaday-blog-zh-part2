# Hackaday 奖参赛作品:开源脉搏血氧仪

> 原文：<https://hackaday.com/2015/08/19/hackaday-prize-entry-open-source-pulse-oximetry/>

很有可能你在某个诊所或医生办公室的指尖或耳垂上夹了一个发光的探针。如果你有过，那么你应该熟悉*脉搏血氧测定法*，这是一种廉价的非侵入性测试，旨在测量你的血液携带多少氧气，另外还可以精确计算你的脉搏率。你可以跑到当地的药店或大盒子里买一个大约 25 美元的指尖脉搏血氧仪，但如果你想了解更多关于光电容积描记术(PPG)，[Rajendra Bhatt]的[开源脉搏血氧仪](https://hackaday.io/project/7177-easy-pulse-plugin)可能是更好的选择。

PPG 是基于氧合血红蛋白和脱氧血红蛋白具有不同光学特性的事实。一个带 LED 的简单探针用红外线照射你的指尖，一个光电二极管读取血红蛋白反射的光量。[Rajendra]的 Easy Pulse 插件接收并放大来自探头的信号，并将其发送到适合 Arduino 使用的接头。你如何处理来自那里的信号取决于你——随着你的心跳及时点亮 LED，绘制氧饱和度与时间的函数关系，或者驱动显示器显示当前的脉搏和饱和度。

我们之前已经见过一些[非常精巧的 DIY 脉搏血氧计](http://hackaday.com/2010/05/02/diy-pulse-oximeter/)，还有一些[具有明显的自制感](http://hackaday.com/2013/04/18/pulse-oximeter-from-lm324-led-and-photodiode/)，但这似乎是复杂设计和开源黑客能力之间的良好平衡。别忘了红外发光二极管也可以用于[其他非侵入性诊断](https://hackaday.io/project/5508-nirgm-non-invasive-nir-glucose-meter)。

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)