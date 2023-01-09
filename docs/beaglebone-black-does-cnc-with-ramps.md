# BeagleBone 黑做数控与坡道

> 原文：<https://hackaday.com/2013/09/19/beaglebone-black-does-cnc-with-ramps/>

[Bart]想试着用他的 BeagleBone black 控制一个 CNC，但是不想投资一个 CNC 斗篷。没问题—[他为 RAMPS](http://www.buildlog.net/blog/2013/09/cnc-translator-for-beaglebone/) 创建了自己的翻译板。[beagle bone Black 的 LinuxCNC](http://beagleboard.org/project/LinuxCNC/) 已经上市几个月了，[巴特]想试一试。他开始用单个步进电机和驱动器进行实验。当他连接起步伐、方向和运动相位时，[Bart]知道他需要一个更好的解决方案。

几个数控斗篷可用于 BeagleBone 板，但[巴特]有一个坡道板只是坐在那里，等待一个新的项目。大多数 RepRap 粉丝都听说过 RAMPS——或 [Reprap Arduino Mega Pololu 盾](https://ultimachine.com/ramps)。事实上，[几天前我们在这里](http://hackaday.com/2013/09/06/3d-printering-electronics-boards/)报道了它们，作为我们 [3D 打印系列](http://hackaday.com/?s=3d+printering)的一部分。RAMPS 处理 3D 打印所需的所有 I/O，这也可以很好地应用于其他 CNC 应用程序。缺点是它们是专门为 Arduino Mega 系列设计的。

翻译板将所有的 BeagleBoard 黑色 IO 信号带到 RAMPS 期望的地方。[Bart]还没有完成，他还增加了 grblShield 和并行端口连接的兼容性。

我们想了解更多的一点是 3.3V 至 5V 电压转换。RepRap 已经开始研究 [RAMPS-FD](http://reprap.org/wiki/RAMPS-FD) 来处理 Arduino Due 的 3.3V 要求。重用硬件是很棒的——我们不想冒险炸掉一只比格犬骨来做这件事。

[https://www.youtube.com/embed/nmt5zrdJukk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/nmt5zrdJukk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)