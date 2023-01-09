# 黑客日奖参赛作品:非常非常小的逻辑

> 原文：<https://hackaday.com/2015/06/04/hackaday-prize-entry-very-very-small-logic/>

尽管有 FPGAs 和 CPLDs 的存在，仍然需要非常小的可编程逻辑器件。不过，GALs、PALs 和其他旧技术无法满足我们的需求，因此我们只能使用新一代可编程设备，而不是微控制器或 CPU。Silego 的 GreenPAC 很好地填补了这一空白，能够在单个芯片上实现计数器、ADC、逻辑胶、电平转换和比较器。对于任何自制电子产品的修补者来说，这些设备都有一个非常明显的问题:它们真的非常非常小。最小的 GreenPAC 设备将 12 个引脚塞入 1.6 x 1.6mm 毫米的 QFN 封装中。你不能手工焊接这个东西。

对于[Nick Johnson]的 Hackaday 奖参赛作品，他正在使用这些小型可编程逻辑芯片[并使创建您自己的定制 IC](https://hackaday.io/project/5805-fabric8)变得容易。基本上，它是一个 GreenPAC 设备的分线板，将这些微小的芯片填充到一个更合理的 DIP 封装中。

突破是不够的，为了对这些小芯片进行编程，[Nick]还在构建一个基于 ARM 微控制器的电路板。通过 USB 输入，一种产生用于编程的 7.5V 电压的方法，以及一种试验板友好的格式，这个程序员将告诉这些微小的芯片做什么。

没有多少人再和朋友或女孩一起做东西了，但是仍然有很多工作可以用小的可编程芯片来完成。像这样的微型可编程逻辑芯片肯定有一席之地，在我们看来，任何能让更多人拥有它们的东西都是可以的。

* * *

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)