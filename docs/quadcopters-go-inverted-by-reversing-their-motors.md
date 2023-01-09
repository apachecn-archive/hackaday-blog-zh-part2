# 四轴飞行器通过反转它们的马达来反转

> 原文：<https://hackaday.com/2013/11/26/quadcopters-go-inverted-by-reversing-their-motors/>

倒四轴飞行器？这通常意味着崩盘即将到来。对于新一代四轴飞行器来说，情况并非如此。这些新的四轴飞行器能够持续倒飞。我们在 hackaday 之前已经看过[倒置四轴飞行器](http://hackaday.com/2012/02/24/variable-pitch-quadrocopter-flies-upside-down/)。然而，以前的倒四轴飞行器总是使用[总距](http://en.wikipedia.org/wiki/Helicopter_flight_controls#Collective)来控制叶片产生的推力。四轴飞行器的总距比传统直升机的主旋翼要简单得多。遥控和全尺寸直升机混合了总距和周期距来铰接主旋翼桨叶。四轴飞行器只需要总距部分，类似于传统的直升机尾桨机构，或者飞机上的变距螺旋桨。

这些新的四轴飞行器使用一种更简单的倒飞方法:向后旋转马达。四轴飞行器通过快速改变每个马达的转速来控制它们的飞行。那为什么不完全反转马达呢？今天的无刷 outrunner 电机有足够的权力来迅速扭转方向。问题变成了一个螺旋桨。标准螺旋桨的设计只能产生一个方向的推力。每架四轴飞行器都使用两个顺时针旋转和两个逆时针旋转的螺旋桨。如果向后旋转，螺旋桨将产生反向推力，但是它们将不会像旋转时设计的方向那样有效。quad fliers 已经找到了这个问题的部分解决方案:从叶片上去掉曲线。遥控螺旋桨叶片按直径和[叶片间距](http://en.wikipedia.org/wiki/Blade_pitch)出售。桨距是叶片攻角的量度。遥控叶片也有一个翼型曲线塑造成他们。去除这条曲线(但不改变音高)有助于解决这个问题。

最后一个问题是控制系统。由于四轴飞行器已经依赖于计算机控制进行基本飞行，所以只需在你的飞行板上加载[定制固件](https://github.com/c---/MultiWii3D)来支持电机反转。速度控制也必须能够反向旋转，这意味着[新固件以及](http://www.rcgroups.com/forums/showthread.php?t=1849952)。我们很好奇四轴飞行器社区是如何决定倒飞的控制系统的。多年来，遥控直升机团体经历了几次控制系统的迭代。在某一点上，他们使用“反转开关”来反转控制以及处理集体音高变化。随着时间的推移，这些开关失宠了，现在被称为“紧急开关”，因为在飞行中或发动机启动前偶然碰到了一个开关。

[https://player.vimeo.com/video/61127136](https://player.vimeo.com/video/61127136)[https://player.vimeo.com/video/67994318](https://player.vimeo.com/video/67994318)[https://player.vimeo.com/video/62015977](https://player.vimeo.com/video/62015977)

【感谢马克】