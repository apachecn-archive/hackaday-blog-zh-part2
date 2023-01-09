# 本周失败:GPS 模块设计

> 原文：<https://hackaday.com/2013/09/05/fail-of-the-week-gps-module-design/>

在你的项目中使用 GPS 真的很有趣。但是当[Trax]决定在他的设计中内置 GPS 芯片时，这种乐趣就戛然而止了。上面你可以看到电路板的硬件部分。不幸的是，这个 PCB 无法提供任何 GPS 定位数据。

他的设计在 Venus634FLPx GPS 接收器和天线之间使用了一个低噪声放大器。填充电路板后，他没有得到卫星定位。他尝试更换天线，并在不使用 LNA 的情况下连接两个不同的天线。他可以得到 NMEA 的数据，但仍然没有修复。经过反复检查，他终于向芯片制造商寻求建议。他们带回来一些有用的建议，但他陷入了试图找出他的天线是否有问题的困境，并且需要旋转另一个 PCB 来测试一些提议的修复。[看看他的文章](http://www.elektronika.ba/649/mobile-robot-platform-v1/)，如果你看到他可能遗漏了什么，请留下评论。

甚至使用开发板 GPS 硬件也有它的起伏。[杰里米·布卢姆]试图跟踪他的财产，因为他们被转移到全国各地的豆荚集装箱。作为一个失败的一周额外节目，看看[他匆忙组装的跟踪硬件是如何在经过凌日的最初几个小时后](http://www.jeremyblum.com/2013/08/31/pod-tracker/)失效的。

* * *

**[![2013-09-05-Hackaday-Fail-tips-tile](img/4ddcb45ba24697ecb36e5a2da073e8dc.png)](mailto:tips@hackaday.com?Subject=[Fail of the Week]) 每周失败是一个每周三运行的黑客专栏。通过写下你过去的失败和[给我们发送一个故事的链接](mailto:tips@hackaday.com?Subject=[Fail of the Week])，或者发送你在互联网旅行中发现的失败报道的链接，来帮助保持乐趣。**