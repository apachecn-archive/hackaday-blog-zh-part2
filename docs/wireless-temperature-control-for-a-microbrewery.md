# 微酿酒厂的无线温度控制

> 原文：<https://hackaday.com/2013/04/04/wireless-temperature-control-for-a-microbrewery/>

[![Wireless Temperature Control](img/12d51e99e881eafd563fac82873efb48.png)](http://hackaday.com/?attachment_id=97322)

酿造自己的啤酒时，温度控制很重要。如果温度调节不当，酵母在加入麦芽汁时会被杀死。加入酵母之前，最好将煮沸的麦芽汁快速冷却到 25°C 左右。

为了做到这一点，[卡勒]为他的家庭酿造设备设计了一个无线温度控制器。该设备使用[热交换器](http://en.wikipedia.org/wiki/Heat_exchanger "Heat Exchanger")冷却麦芽汁。连接到 H 桥的 ATmega88 控制调节通过热交换器的流量的阀门。它从 LM35 温度传感器读取当前温度，并驱动阀门将麦芽汁带到设定点。

一个整洁的建筑是一个无线电台。 [nRF24L01](http://www.nordicsemi.com/eng/Products/2.4GHz-RF/nRF24L01 "nRF24L01") 模块提供与计算机的无线连接。有一个 Android 应用程序可以与电脑通信，提供温度监测，并在任何[卡勒]可以连接互联网的地方控制设定点。