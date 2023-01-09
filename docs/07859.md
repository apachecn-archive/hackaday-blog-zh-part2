# 电子手套检测手语

> 原文：<https://hackaday.com/2014/12/20/electronic-glove-detects-sign-language/>

康奈尔大学的一个学生小组最近制作了一个电子手套原型，它可以检测手语并大声说出手语字符。该手套设计用于各种尺寸的手，但目前只适合右手。

这种手套使用几种不同的传感器来检测手的运动和位置。也许最明显的是覆盖每个手指的柔性传感器。这些传感器可以通过根据弯曲程度改变电阻来检测每个手指是如何弯曲的。该手套还包含一个 MPU-6050 三轴加速度计和陀螺仪。这个传感器可以检测手的方向和旋转运动。

虽然更高科技的传感器用于检测大多数字符，但有几个字母非常相似，足以欺骗系统。具体来说，他们对字母 R、U 和 v 有困难。为了解决这个问题，学生们有策略地在手指的几个位置放置了铜带。当两片胶带碰到一起时，它就会闭合电路，充当瞬时开关。

传感器数据由 ATmega1284p 微控制器收集，然后编译成数据包。这个包被发送到一台 PC 机，然后由它进行繁重的处理。该系统使用机器学习算法。用户可以通过多次对字母表中的每个字母做手势来训练它。该系统将收集所有这些数据，并将其存储到一个数据集，然后可用于检测。

这是一个很好的项目。如果你需要更多的灵感，有很多可以找到，包括另一个康乃尔的项目，即[说出你签署的字母](http://hackaday.com/2012/05/04/sign-and-speak-glove/)，以及[这个将所有需要的部件绑在你的前臂上](http://hackaday.com/2010/10/04/from-sign-language-to-spoken-language/)。

[https://www.youtube.com/embed/f1lSoTNKzfQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/f1lSoTNKzfQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)