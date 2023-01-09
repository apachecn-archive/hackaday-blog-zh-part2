# 借助宜家和 ESP8266，互联网了解你的一举一动

> 原文：<https://hackaday.com/2015/03/29/internet-knows-your-every-move/>

[terenceang]尝试使用 ESP8266 WiFi 模块，组装了一款宜家 Molgan PIR 灯。当检测到运动时，stock PIR 灯简单地点亮。[terenceang]给它添加了一些额外的功能，让它也能向自己的手机发送通知。

库存 PIR 灯的默认配置是只在夜间工作。这是用光电二极管完成的。它和其他几个部件一起被移走，以便在白天工作。他移除了一些限流电阻，以禁用 hi 输出 led。一个被保存下来作为视觉指示器。机载电压调节器没有为 ESP8266 提供足够的电流。[泰伦桑]使用了一些电子魔法，用光耦合器解决了这个问题。

他将改变的一件事是从电池转向主电源，因为预计电池寿命不到两周。原理图，源代码和大量的图片都可以在他的博客上找到。如果你想尝试一下，但需要一个速成班，请查看最近的[新闻，Arduino IDE 可与 ESP8266](http://hackaday.com/2015/03/28/arduino-ide-support-for-the-esp8266/) 或[一起工作，尝试直接编程](http://hackaday.com/2015/03/18/how-to-directly-program-an-inexpensive-esp8266-wifi-module/)。