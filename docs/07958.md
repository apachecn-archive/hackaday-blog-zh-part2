# ESP Lua 解释器的开发板

> 原文：<https://hackaday.com/2015/01/01/a-dev-board-for-the-esp-lua-interpreter/>

ESP8266 的 NodeMCU Lua 解释器背后的伟大智慧为 2015 年的 WiFi 平台提供了合适的开发板。他们称之为 NodeMCU-devkit，这是一款适用于 ESP8266 的合理、廉价且可在电路板上安装的分线板。

本项目中使用的 ESP8266 版本是 ESP-12，这是一款更新、更精致的型号，带有 RF 屏蔽、可疑的 FCC 徽标，并且每个 GPIOs 都暴露在齿形连接器上。电路板的其余部分是一个 USB 转串行转换器(ch 340g-[可能是最便宜的 USB 转串行芯片](http://hackaday.com/2014/12/02/finding-a-cheaper-usb-to-serial-chips/))、几个无源器件和一个 USB 微型连接器。它简单、便宜，而且是开源的。你不能做得比那更好。

该开发板专门设计用于与 [NodeMCU 固件](https://github.com/nodemcu/nodemcu-firmware)协同工作，后者是一种基于 Lua 的 ESP 固件。我们已经看到一些项目[用这个固件制作了 Hackaday 首页](http://hackaday.com/2014/11/23/using-the-esp8266-as-a-web-enabled-sensor/)。当然，这只是一个车库开门器，但对于一个只有几个月历史的芯片来说，这是非常令人印象深刻的。

谢谢[狒狒]的提示。