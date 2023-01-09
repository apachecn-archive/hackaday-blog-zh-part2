# 使用 ESP8266 跟踪比特币

> 原文：<https://hackaday.com/2015/06/18/tracking-bitcoin-with-the-esp8266/>

[Kendrick]正在寻找与 ESP8266 WiFi 模块有关的东西，由于他喜欢比特币和 Arduino，显而易见的解决方案是让[成为比特币价格追踪器](http://www.kendricktabi.com/2015/06/bitcoin-price-ticker-using-esp8266-wifi-module.html)。

ESP8266 是一个完整的微控制器，带有一个 WiFi 芯片和几个串行连接引脚。当然可以为 ESP 编写一些固件来获得比特币的当前转换率，但为了简单起见，[Kendrick]选择为这个项目使用一个 Arduino。他使用 5V Arduino，ESP 在 3.3V 逻辑上运行，但少数 Zeners 负责逻辑电平转换。

Arduino 上运行的代码检查 [CoinDesk API](http://www.coindesk.com/api/) 分钟，解析来自 API 的 JSON，并将当前比特币价格打印到串口。对于追踪比特币当前的转换率来说，这是大材小用。这个项目可能有一些有趣的应用，从连接几个七段显示器，到跟踪这笔神奇的互联网资金的 RGB LED 情绪灯。