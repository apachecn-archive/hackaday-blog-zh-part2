# 蓝牙低能耗气象灯

> 原文：<https://hackaday.com/2013/08/30/bluetooth-low-energy-weather-lamp/>

![bluetooth_low_energy_ble_weather_lamp](img/256af83756c52bee24b7fb1aed5f479f.png)

这是[Aaron Jeromin]在几个小时内完成的概念证明。这盏灯拥有一个蓝牙低能耗天气显示器。这个项目是他习惯使用 BLE 模块的一种方式。但是，为了充分利用该硬件，应该将其改进为一个真正的低功耗电路。我们确实认为现在是展示这个项目的最佳时机，因为[我们昨天刚刚看了一部 BLE 的初级读本](http://hackaday.com/2013/08/29/primer-on-bluetooth-low-energy/)。

他用的是 RedBearLab 的 BLE 迷你板。它使用德州仪器 CC2540 SoC。我们很希望看到一个废除 Arduino 的后续产品，取代 TI 芯片上运行的代码。但是我们会在第一次测试 BLE 板时做同样的事情(使用我们最熟悉的 uC)。它从 iPhone 上获取天气数据。天气预报通过一个 LED 灯泡和一个由业余爱好伺服系统定位的模板被投射成三个图标中的一个。

其他可以告诉你是否正在暴风雨中的无生命物体包括这个颜色编码的伞架。

[https://www.youtube.com/embed/8SyWbO49g38?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/8SyWbO49g38?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)