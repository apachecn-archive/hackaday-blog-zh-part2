# 集成了仪表板显示屏和方向盘控制的雷达探测器

> 原文：<https://hackaday.com/2013/08/31/radar-detector-integrated-with-dashboard-display-screens/>

CAN 总线黑客现在非常流行。这个特殊的项目使用 Arduino 兼容 CAN 总线工具的早期开发版本[将雷达检测器控制集成到马自达仪表板](http://phzero.net/?q=whistler)。此图显示了 Whistler Pro-3600 雷达探测器启动时的输出。自检演示了如果使用少数几种技术中的任何一种来检查您的速度，您会在仪表板显示屏上看到什么。但不仅仅是仪表盘显示在起作用。方向盘控制也能够影响雷达探测器，使其始终隐藏在视线之外。

随着汽车制造商在我们的汽车上增加更多更大的显示屏，看到有人想出一种黑客技术，使得将我们自己的信息推送到这些屏幕上成为可能，这令人耳目一新。CANBus Triple 是一种 Arduino 兼容板，可插入所有现代车辆中的数据总线。为了将 Whistler 集成到这次攻击中，[TheDukeZip]在一个常规 Arduino 板上制作了接口原型，然后在它工作后将其转移到 CANBus Triple 上。休息之后，请观看视频，了解实际设置。

[https://www.youtube.com/embed/2bSiRKTtazo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/2bSiRKTtazo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[感谢兰迪通过[马自达速度论坛](http://www.mazdaspeedforums.org/forum/f434/introducing-canbus-triple-150523/)