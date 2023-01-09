# 旨在取代卤素灯的调光 LED 灯泡

> 原文：<https://hackaday.com/2013/06/28/dimming-led-bulbs-designed-to-replace-halogen-lamps/>

卤素灯泡发出大量的聚焦光，但这是以消耗大量瓦特和产生大量热量为代价的。像上面看到的拆卸的 LED 更换的成本已经下降了不少。这促使[乔纳森·富特]购买了几台设备，他忍不住把它们拆开来试了几个。

我们发现最有趣的是[他用 Arduino 板和 FET 实现的基于 PWM 的调光技术](http://rotormind.com/blog/2013/Dimming-a-LED-Lamp-with-an-Arduino/)。灯泡被设计成可以通过给灯具供电的 12V 电源进行调光。但是调光器的位置和亮度的关系不是线性的，乔纳森认为他可以做得更好。他的解决方案是增加一个与 led 并联的 FET。当激活时，它基本上分流二极管周围的电流，导致变暗。下面的视频展示了这一点。我们想知道闪光是不是相机的伪影，还是你也用眼睛看到的？

你可能也有兴趣阅读他关于[胶凝 LED 灯泡](http://rotormind.com/blog/2013/Gelling-a-LED-Lamp/)的帖子。凝胶是光线(或相机镜头)的彩色滤光片。他将自己喜欢的颜色切割成合适的尺寸，并将其插入发光二极管和透镜之间。

[https://embedr.flickr.com/photos/9091073880](https://embedr.flickr.com/photos/9091073880)