# 将 ESP8266 用作网络传感器

> 原文：<https://hackaday.com/2014/11/23/using-the-esp8266-as-a-web-enabled-sensor/>

几个月前，ESP8266 作为一种廉价的方式出现，几乎可以为任何有备用 UART 的项目添加 WiFi。从那以后，一些人已经想出了如何让这个整洁的芯片运行定制固件，打开了基于 ESP8266 的物联网的大门。[Marc]和[Xavi] [刚刚撰写了一篇快速教程](http://importhack.wordpress.com/2014/11/22/how-to-use-ep8266-esp-01-as-a-sensor-web-client/)，介绍如何将 ESP8266 转变为 WiFi 传感器平台，将 GPIO 引脚的状态转发到互联网。

如果您要复制这个项目，您将不会在 ESP 上使用现有的固件。[Marc]和[Xavi]没有使用普通固件，而是使用基于 Lua 的固件,该固件允许访问设备上的一些 GPIOs 和脚本支持，从而简化应用程序开发。为了将该固件上传到 ESP，[Marc]和[Xavi]需要一个标准的 FTDI USB 转串行转换器、一些通过终端程序的 AT 命令和一些电线。

circuit [Marc]和[Xavi]在本教程中演示的是一个简单的网页，每次按下按钮都会更新。这将被安装在巴塞罗那他们的黑客空间的门口，但是他们已经有了一个正在使用的 ESP8266 的很好的例子。