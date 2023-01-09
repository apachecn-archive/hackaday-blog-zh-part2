# Hackaday 奖参赛作品:双组分温度传感器

> 原文：<https://hackaday.com/2015/06/12/hackaday-prize-entry-a-two-component-temperature-sensor/>

这里有一个设计挑战:为任何计算机制造一个温度传感器。如果你非常聪明，你可能会写一些代码来报告 CPU 的温度。其他认真对待这项工作的人可能会用一个单线温度传感器、一个微控制器和所有需要的硬件来建造一些东西。

[迈克尔]有一个更好的主意。他只用了两个组件就做到了。其中一个组件是 USB 连接器。

唯一可以创建项目的原因是 Microchip 的一个相当新的部件，PIC16F1455。这个微控制器不需要一个晶体，不需要任何额外的部件就可以做 USB，并且集成了温度传感器。[迈克尔]迅速完成了一个项目，建立一个 USB CDC 串行设备，用 ADC 读取温度(感谢[一个非常有用的应用程序注释](http://ww1.microchip.com/downloads/en/AppNotes/01333A.pdf))，并每秒一次将温度发送到计算机。

尽管只由两个组件组成，这实际上可能是一个有用的设备。PIC 是一个 USB 串行设备，它可以用于过去 15 年左右生产的任何计算机。用另一个程序读取温度几乎不需要任何代码，而且这是一个非常便宜的构建。我们还必须给出将微控制器直接焊接到 USB 连接器的风格要点。

* * *

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)