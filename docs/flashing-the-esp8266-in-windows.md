# 在 Windows 中刷新 ESP8266

> 原文：<https://hackaday.com/2015/01/10/flashing-the-esp8266-in-windows/>

ESP8266 在中国的一些工厂推出才几个月，社区已经从简单地让定制固件在设备上工作转向使开发工具易于使用。这是巨大的——进入的门槛降低了，让更多的人参与到这个非常酷的物联网事物中来。

虽然社区的大多数人已经决定使用 Lua 解释器固件，但是仍然有将这个固件上传到 ESP 的问题。Microchess fame [的【Peter Jennings】一直在开发一款 Windows 应用](http://benlo.com/esp8266/index.html#LuaLoader)，通过串行接口向 ESP 上传固件。没什么大不了的，但这将允许你上传[社区创建的 Lua 固件](https://github.com/nodemcu/nodemcu-firmware)，设置 WiFi 凭证，切换 GPIO 引脚，并让你能够在同一个窗口中编写一点点 Lua。

如果你在寻找不是专为 Windows 设计的东西，nodemcu Github 上有一个替代的固件 flasher】。该闪光器还将 ESP8266 连接到网络并上传固件。这是一个精简的编程器，没有串行终端或切换引脚的能力，但有计划使这种编程器跨平台。