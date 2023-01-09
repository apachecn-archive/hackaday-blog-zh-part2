# 皮尤皮尤！基于 Arduino 的激光测距仪

> 原文：<https://hackaday.com/2014/07/01/pew-pew-an-arduino-based-laser-rangefinder/>

激光器是最酷的设备之一。我们可以用它们来切割东西，制作激光表演，也可以作为测距仪。[Ignas]写信告诉我们[berry jam]关于创造一个基于 [Arduino 的激光测距仪](http://www.berryjam.eu/2014/06/oslrf-01/)的惊人报道。这个帖子绝对值得一读。

受到一个基于 Arduino 的激光雷达系统的启发，[Berryjam]决定成功使用一个来自 [LightWare](http://www.lightware.co.za/) 的廉价开源激光测距仪(OSLRF-01)。这篇文章从如何用基于激光的系统测量距离的基础知识开始。你测量一个输出激光脉冲和反射回来的脉冲之间的时间；这个时间直接关系到物体的距离。听起来很简单？实际上，这并不像看起来那么简单。[Berryjam]在对这款设备进行真实世界测试方面做得很好，有很好的情节来完成这一切。在修改了阈值和代码的一些其他方面之后，结果的准确性相当好。

最近，我们看到了更多利用激光进行测距的项目，包括[激光雷达项目](http://hackaday.com/2014/01/23/lidar-with-leds-for-under-100/)。看到这样的高端传感器进入制造商/黑客领域是非常令人兴奋的。如果你有相关的激光项目，一定要[让我们知道](http://hackaday.com/contact-hack-a-day/)！