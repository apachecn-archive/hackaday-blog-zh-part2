# ESP8266 的 Arduino IDE 支持

> 原文：<https://hackaday.com/2015/03/28/arduino-ide-support-for-the-esp8266/>

尽管有大量关于为 ESP8266 WiFi 模块设置和编写代码的教程，但还没有多少关于用 Arduino IDE 对这种廉价的无线模块进行编程的内容。终于，这种情况改变了。经过数月的编码，[Arduino IDE 支持 ESP8266 模块](https://github.com/esp8266/arduino)。

Arduino IDE 支持在 [ESP8266 社区论坛](https://github.com/esp8266/arduino)上宣布。对于 Linux、OS X 和 Windows，安装非常简单。这也不是 ESP8266 屏蔽:您可以为 ESP 模块编写代码，连接串行引脚，然后点击 program 按钮。

Arduino IDE 的基本功能(pinMode、digitalRead、digitalWrite 和 analogRead)可用。大部分 WiFi 功能的工作原理和 WiFi 盾库一样。

有几件事还没写出来；PWM 不起作用，因为 ESP8266 只有一个硬件 PWM 源。SPI 和 I2C 奴隶模式还没有完成，通过 WiFi 上传草图需要一点点思考。也就是说，这是对 ESP 模块编程的一个很好的介绍。如果你不喜欢 Arduino IDE，你可以用我们上周特别介绍的[【CNLohr】的编程教程](http://hackaday.com/2015/03/18/how-to-directly-program-an-inexpensive-esp8266-wifi-module/)来酷一把。