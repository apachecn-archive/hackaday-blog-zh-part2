# 双轴太阳能跟踪器

> 原文：<https://hackaday.com/2015/08/25/two-axis-solar-tracker/>

太阳能电池板是一项令人惊叹的工程，但是如果没有合适的条件，它们会变得非常不稳定。最重要的条件之一是电池板必须指向太阳，电池板的精确瞄准可以通过太阳能跟踪器来完成。太阳能跟踪器可以大幅提高太阳能电池板的能量收集能力，现在[Jay]有了一个也是便携式的双轴跟踪器。

这个项目的核心是一个 Raspberry Pi，选择它是因为[Jay]发现 Arduino 没有足够的内存来实现他想要的所有功能。Pi 和电机控制电子设备被塞进一个鹈鹕箱中，以防风雨。实际的太阳跟踪完全是在软件中完成的，只需要一个纬度和经度就可以知道太阳在哪里。这比依靠 GPS 或光学系统获取太阳位置信息要容易得多(也便宜得多)。

一定要看看下面的太阳能跟踪器的视频。即使没有电池板(或太阳，就此而言)，追踪器也能够精确定位电池板，以获得最大的能量效率。而且，如果你想从太阳能电池板获得更多的能量，你也应该试试最大功率点跟踪系统。

[https://www.youtube.com/embed/fOk4_Ym5IXU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/fOk4_Ym5IXU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)