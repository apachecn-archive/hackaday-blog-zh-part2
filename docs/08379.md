# 可穿戴 WiFi Finder 使用 ESP8266

> 原文：<https://hackaday.com/2015/02/22/wearable-wifi-finder-uses-the-esp8266/>

在 Hackaday 上，似乎没有一天没有 ESP8266 项目。有一个很好的理由，芯片和相关模块为大众带来了低成本的 WiFi 连接。今天我们请来了【Stevica Kuharski】，她[使用 ESP8266 构建了一个开放式 WiFi 接入点检测器](https://medium.com/@kstevica/how-to-build-an-open-wifi-finder-using-esp8266-and-two-coin-batteries-9c31eb6f9859)。为此，他使用了 [Lua 兼容节点 Mcu 固件](https://github.com/nodemcu/nodemcu-firmware)。[Stevica]编写了自己的 Lua 脚本，在 ESP8266 的内部 32 位微控制器上运行。freewifi 脚本扫描并搜索开放的 wifi 网络。如果检测到网络，将通过闪烁的 LED 通知用户。

为了使该项目可穿戴，[Stevica]为该项目提供了一对 CR2450 纽扣电池。ESP8266 并不是一个特别低功耗的设备，所以我们很想知道[Stevica]在他的项目中获得了什么样的电池寿命。这个项目的源代码已经可以在 [GitHub、](https://github.com/kstevica/ESP8266-WiFi-Finder)上获得，并且【Stevica】希望在接下来的几周内启动一个 Indiegogo 活动。点击休息时间，查看 WiFi 检测器的运行情况。

[https://player.vimeo.com/video/120285238](https://player.vimeo.com/video/120285238)