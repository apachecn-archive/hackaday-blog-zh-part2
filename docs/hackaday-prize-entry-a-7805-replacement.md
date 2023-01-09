# Hackaday 奖品入口:7805 替代品

> 原文：<https://hackaday.com/2015/05/13/hackaday-prize-entry-a-7805-replacement/>

如果你想用简单的方法把电压降到 5V，7805 电压调节器是一个很好的设备。这是一种三引脚、单组件解决方案，可产生 5 伏电压和大量热量。简单，不高效。为了他的 Hackaday 奖参赛作品，[K.C. Lee] [正在开发一种更高效的替代 7805](https://hackaday.io/project/2145-smps-replacement-for-7805) 的小型车。

像 7805 这样的线性调节器很好，但它们的效率不是很高。根据输入电压，你*可能*看到 50%的效率。使用开关模式电源，效率可高达 90%左右。

对于他的替代产品，[K.C. Lee]正在使用 [LM3485](http://www.ti.com/product/LM3485?keyMatch=lm3485&tisearch=Search-EN) ，这是一种开关模式调节器，只需要一些额外的部件就可以将其变成 7805 的替代品。输入端需要一个电容，但无论如何，你应该已经把电容放在电路中了，对吧？

* * *

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)