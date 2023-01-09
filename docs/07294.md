# 使用 BrewMonitor 监控您的发酵啤酒

> 原文：<https://hackaday.com/2014/10/11/keep-an-eye-on-your-fermenting-beer-with-brewmonitor/>

酿造啤酒的艺术和文明本身一样古老。许多人喜欢在家自己酿造啤酒。在你痛饮之前，必须采取许多步骤，但发酵是最关键的步骤之一。[Martin Kennedy]和他的朋友一起开始了这项爱好，他想要一种方便的方法来远程监控发酵温度。他开始研发 brew monitor T1，这是一款基于云的家庭酿酒控制器，由 Arduino 克隆产品驱动。

他的目标是创造一些便宜、方便、易于安装的东西。传统的发酵监控设备非常昂贵。典型的开源替代方案将花费你 80 欧元(大约 101 美元)，通过 [BrewPi](http://hackaday.com/2012/10/01/brewpi-is-a-raspberry-pi-in-charge-of-beer-fermentation/ "BrewPi article") 网络服务器使用 Arduino-sensor 和 Raspberry Pi 网关。[Martin]不想经历远程查看 BrewPi 的麻烦，因为它需要一个家庭网络和所有必要的配置。相反，他将一个 [Arduino 克隆](http://www.dx.com/p/diy-funduino-uno-r3-development-board-microcontroller-w-usb-cable-240588#.VDi_mBZeJEM "Funduino Uno")与一个 [DS18B20 温度传感器](http://www.adafruit.com/product/381 "DS18B20 Temperature Sensor from Adafruit")结合在一起，同时使用一个 [ESP8266 模块](https://nurdspace.nl/ESP8266 "ESP8266 Wireless Module")进行无线通信，所有这些花费不到 18 欧元(23 美元)。它连接到一个基于 Scotch.io 的简单网页，带有一个 PHP 后端(带有 RESTful API 的 Laravel)、一个 MySQL 数据库和一个 AngularJS 前端来显示图形。一旦传感器被放入发酵桶的[热电偶套管](http://en.wikipedia.org/wiki/Thermowell)，温度每分钟被传输一次到 REST API。[可以看到一段时间内的温度](http://dev.thebedroomlaboratory.com/~martin/brewmonitor/ "BrewMonitor Temperature Page")(以摄氏度为单位)。设计文件可在 [GitHub](https://github.com/thebedroomlaboratory/BrewMonitor "GitHub link to the BrewMonitor design files") 上获得。

[Martin]希望扩展 BrewMonitor 的功能，例如添加通过控制加热器或冰箱来远程调节温度的功能，以及通过单板化来降低成本。由于信息存储在云上，升级系统比使用单独的网关设备容易得多。他不排除未来的众筹活动。我们希望看到这一点得到进一步发展，因为不同的酵母种类和啤酒风格需要非常严格的条件，特别是在长达数周的发酵过程中；5 摄氏度的温差可以毁掉一整杯啤酒。基于云的温度调节似乎是 BrewMonitor 的下一个大目标。DIY 酿酒师向你致敬，[马丁]！

[via [危险原型](http://dangerousprototypes.com/2014/10/03/brewmonitor-the-arduino-powered-cloud-based-homebrewing-controller/ "Dangerous Prototypes- BrewMonitor")