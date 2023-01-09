# 使用 ESP8266 无线称重设备

> 原文：<https://hackaday.com/2015/06/28/wirelessly-weighting-plants-with-the-esp8266/>

有很多黑客和商业产品会告诉你什么时候植物需要浇水。大多数使用 ADC 来测量土壤中的电阻。随着土壤含水量的下降，阻力增加。高阻抗，死植物。

[squix]的 [Thirsdee](http://blog.squix.ch/2015/06/esp8266-meet-thirsdee-intelligent-plant.html) 采用不同的方法来监测工厂的健康状况。它不是测量电阻，而是简单地称植物的重量。随着土壤变干，它变轻了。通过测量重量的变化，可以估算出锅里的水量。

Thirsdee 使用称重传感器测量重量。使用由[节点 MCU](http://nodemcu.com/index_en.html) 控制的 [HX711](https://learn.sparkfun.com/tutorials/load-cell-amplifier-hx711-breakout-hookup-guide) ADC 读取。该开发板基于 ESP8266 芯片。由于 Thirsdee 有 WiFi，它可以向你的手机推送通知，并在 [ThingSpeak](https://thingspeak.com/) 上记录数据。如果你在看植物，有机发光二极管会显示植物的当前状态。对于在家观看的我们来说，我们可以看到[squix]的植物正在实时变干的图表。

[squix]为我们提供了零件的供应商名单，以及 [Github](https://github.com/squix78/esp8266-projects/tree/master/arduino-ide/thirsdee) 上的所有源代码。