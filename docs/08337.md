# 天哪！通量电容器通知灯

> 原文：<https://hackaday.com/2015/02/17/great-scott-a-flux-capacitor-notification-light/>

如果你喜欢你的社交媒体，那么你可能喜欢随时更新你的通知。[Gamaral]有这种感觉，但他不喜欢查看网站或等待手机提醒的标准方式。他想要更花哨的东西。类似于[通量电容通知灯](https://hackaday.io/project/4323-flux-capacitor-car-charger-iot-hack "Flux capacitor notification light")的东西。这个设备不会及时发送他的信息，但它看起来很酷。

他从一个现成的通量电容 [USB 充电器](http://hackaday.com/2014/11/28/turn-cordless-tool-batteries-into-usb-chargers/ "USB Charger Hacks")开始。通常这个设备只是在给你的 USB 设备充电的时候看起来很酷。[Gamaral]想给自己更多的控制权。他首先打开外壳，更换一个表面贴装电阻。替换元件实际上是一个 3.3V 调节器，其外形恰好与原始电阻相似。这个调节器现在可以为设备本身以及 ESP8266 模块提供稳定的电源。

[ESP8266 模块](http://hackaday.com/2014/12/08/compiling-your-own-programs-for-the-esp8266/ "ESP8266")内置 WiFi 功能，价格低廉。电路板本身也很小，非常适合这个项目。[Gamaral]只使用了两个 GPIO 引脚。第一个开关控制磁通回路的开和关，第二个开关跟踪回路的当前状态。为了实际触发变化，[gamaral]只需通过 TCP 连接到模块，并发出“时间电路开/关”命令。这种简单性使该设备更加通用，因为在 PC 上运行的应用程序实际上可以跟踪各种社交媒体，并相应地刷新该设备。