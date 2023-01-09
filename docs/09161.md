# Hackaday 奖参赛作品:更好的 DIY CT 扫描仪

> 原文：<https://hackaday.com/2015/05/29/hackaday-prize-entry-a-better-diy-ct-scanner/>

如果你参加今年的黑客日奖，彼得·詹森是一个你需要注意的人。去年，他凭借[开源科学三录仪](https://hackaday.io/project/1395-open-source-science-tricorder)获得第四名，今年他将进入[一台自制核磁共振仪](https://hackaday.io/project/5030-low-field-mri)。这两个都是不可思议的例子，说明只需足够的工具就可以在工作台上构建，但即使这些构建也不能涵盖[Peter]构建的所有内容。几年前，【彼得】[造了一台台式 CT 扫描仪](http://hackaday.com/2013/10/23/towards-a-low-cost-desktop-ct-scanner/)。CT 扫描仪工作，但不是很好；这台机器需要九个小时来获取一片柿子椒。以这样的速度，任何蔬菜或水果都会在完整扫描完成前开始腐烂。

这并没有阻止放射学教授和生物医学家的电子邮件潮水般涌入[彼得]的收件箱。有很多人在等待后巷 CT 扫描，但 CT 扫描仪，现在，只是不能胜任这项任务。解决方案是迭代，在 hackaday.io 的放射科，[Peter]正在开始一个新的项目:[一个改进的台式 ct 扫描仪](https://hackaday.io/project/5946-openct2)。

这种 CT 扫描仪的前一版本使用钡检查源——无需许可证即可获得的最热的放射性同位素源——和在[辐射手表](http://www.radiation-watch.org/p/english.html)中找到的光电二极管探测器来扫描小物体。这种来源与探测器不匹配，肯定有数据埋在噪声层之下，但不知何故，它的工作。

对于桌面 CT 扫描仪的这一版本，[Peter]正在寻找提高扫描速度的方法。他提出了三种技术，可以让他进行更快、更高分辨率的扫描。首先是减少扫描量:探测器越靠近源，计数越多。第二个是多重探测器，接下来是比辐射手表更好的探测器。

[Peter]提出的解决方案仍然使用钡检查源，但用多个 PIN 光电二极管取代了大光电二极管。CT 扫描仪中将有十几个传感器，所有传感器都基于 Maxim 应用笔记的[，这种 CT 扫描仪的机械设计大大简化了构建。](http://www.maximintegrated.com/en/app-notes/index.mvp/id/2236)

与[彼得]的第一台 CT 扫描仪的*星际之门*一样的虚构相比，新的非常简单，也应该快得多。那些放射学教授和生物医学家是否会前往[詹森博士]的后巷 CT 扫描店完全是另一个问题，但它仍然是一个惊人的例子，说明激光切割机和 Mouser 的订单可以做什么。

* * *

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)