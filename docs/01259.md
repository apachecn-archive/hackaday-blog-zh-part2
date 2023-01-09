# 带 MSP430 的 POV 自行车车轮

> 原文：<https://hackaday.com/2012/08/06/pov-bike-wheels-with-the-msp430/>

![](img/7298a23235096f6a73f72a84a962af2c.png "TI")

在德州仪器做实习生并不好玩，但从[乔治]、[瓦莱丽]和[瑞安]的德州仪器实习生设计项目来看，看起来确实如此。他们使用曾经流行的 MSP430 Launchpad 板为自行车建造了一个[视觉暂留显示器。](http://e2e.ti.com/group/msp430launchpad/m/project/664376.aspx)

实习生团队通过将 TI Launchpad 的电源与焊接在升压包上的一排 32 个 RGB LEDs 结合起来，创建了一个 POV 显示器。一旦整个电路牢固地固定在自行车车轮上，安装在自行车车架上的霍尔效应传感器就可以让 MSP430 检测到它的速度。从那以后，只需要在合适的时间闪烁发光二极管，就可以在旋转的轮子内创建一个固定的显示。

虽然该显示器理论上只需一个发射台/升压包组合即可工作，但该团队决定使用三个这样的电路，每个轮子总共 96 个 led，来创建一个真正漂亮的 RGB 显示器。视频(休息后可用)显示了一点点闪烁，但这是相机的一个伪像。在现实生活中，POV 自行车车轮显示简直令人震惊。

[https://www.youtube.com/embed/S0hutxTx2NI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/S0hutxTx2NI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)