# 使用 ESP8266 通过 WiFi 对 Arduino 进行编程

> 原文：<https://hackaday.com/2014/11/13/programming-an-arduino-over-wifi-with-the-esp8266/>

许多人已经使用 ESP8266 将廉价的 WiFi 连接添加到他们的项目中，但[Oscar]决定更进一步，用 ESP8266 编程一个基于 WiFi 的 Arduino。[Oscar]用 Python 编写了一个服务器脚本，与 Arduino 上运行的固件进行通信。Arduino 在启动时连接到服务器，并监听“重新启动”命令。

当接收到命令时，处理器复位并进入引导加载程序。python 脚本开始通过 WiFi 将一个十六进制文件传输到 ESP8226，ESP8226 将其转发到 Arduino 的引导加载程序。一旦十六进制文件被流式传输，微控制器就无缝地开始执行固件。该方法可用于任何运行 stk500 兼容引导程序的 AVR。

[Oscar]的文章是西班牙语的，但幸运的是，他的 Python 和 Arduino 代码中的注释是英语的。休息之后，请观看视频(英文版)，其中[Oscar]演示了他的引导安装。

[https://www.youtube.com/embed/JYGhlOkNins?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/JYGhlOkNins?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)