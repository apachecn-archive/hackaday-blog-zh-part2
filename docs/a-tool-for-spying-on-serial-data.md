# 一种监视串行数据的工具

> 原文：<https://hackaday.com/2015/05/06/a-tool-for-spying-on-serial-data/>

[Piotr]在从事最近的 Arduino 项目时遇到了一个问题。他在让他的 Arduino Pro Mini 与 ESP8266 模块通信时遇到了问题。他需要一种方法来窥探来回串行通信。因为他没有完成这项任务的专用工具，所以[Piotr]最终[建造了自己的](http://nicecircuits.com/dual-port-serial-terminal/ "Serial Spying")。

设置非常简单。从包含 TX、RX、DTR 和 GND 线的标准串行电缆开始。这条电缆将 Arduino 连接到 [ESP8266 WiFi 模块](http://hackaday.com/2014/08/26/new-chip-alert-the-esp8266-wifi-module-its-5/ "ESP8266 Wifi Module")。然后，TX 和 RX 线路被接入。每条线都连接到两个不同的串行转 USB 适配器的 RX 引脚。这样，从 Arduino 发送的数据显示在一个 COM 端口上，从模块传输的数据显示在另一个端口上。

下一个难题是想出一种更清楚地查看数据的方法。[Piotr]可以同时打开两个串行终端，但这并不理想，因为很难比较数据的时序。相反，[Piotr]花了不到一个小时编写了自己的简单串行终端。这个可以同时连接两个 COM 端口，并在同一个屏幕上打印数据。来自每个 COM 端口的数据以不同的颜色显示，以便于区分。这个项目的原理图和源代码可以在[Piotr 的]网站上找到。