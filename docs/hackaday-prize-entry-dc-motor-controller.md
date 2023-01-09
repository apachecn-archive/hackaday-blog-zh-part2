# 黑客日奖参赛作品:DC 电机控制器

> 原文：<https://hackaday.com/2015/05/15/hackaday-prize-entry-dc-motor-controller/>

有很多便宜的中国数控机床，机械性能不错，电子性能很差。轴承不完全是垃圾，但这些数控机床的主轴是一个独立的 PWM 控制器，有一个锅来控制速度。这意味着你不能用 LinuxCNC 或 Mach3 控制主轴速度。

作为他的 Hackaday 奖参赛作品，[SUF]正在为一台不使用任何编码器的中国主轴电机制造一个 DC 电机控制器。这个项目第一部分相当容易；【SUF】已经造了一个[大电流驱动](https://hackaday.io/project/1983-high-current-driver)。第二点有点难——因为这些主轴没有编码器，[SUF]必须读取电机磁极上的电压尖峰，给他主轴的转速。从那里，这是一个位的 PID 代码，让这个主轴运行在一个理想的转速，并连接到一个数控控制箱。

到目前为止，【SUF】[已经有了他的第二版主板等待组装](https://hackaday.io/project/2439-dc-motor-controller-for-cnc-router/log/17408-v2-boards)。在电路板的第一个版本中，MOSFET 的开关时间有点慢，但在当前版本中已得到纠正。这是一个扩展这些廉价数控机床能力的伟大项目，也是 Hackaday 奖的完美项目。

* * *

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)