# THP 半决赛:蜜蜂蜂巢监测

> 原文：<https://hackaday.com/2014/09/23/thp-semifinalist-honeybee-hive-monitoring/>

[Ken]将他的蜜蜂放在远处，不能像他希望的那样经常检查它们。他想知道它们何时离开了太空，因为那会减缓它们采集花蜜的速度。他知道他可以通过远程跟踪蜂巢的重量和内部温度来做到这一点。

他的第一个原型围绕着一个不能在读数之间关闭的邮政秤。这意味着他需要比原先计划的更大的太阳能电池板和电池。在大约一周的时间里，蜂巢通过 XBee 上的 Arduino [Fio](http://arduino.cc/en/Main/ArduinoBoardFio) 向 Thingspeak 发送数据。

当前迭代使用 HX711 24 位 ADC 测量称重传感器。这将规模数据发送到 Apitronics 蜜蜂单元，该单元添加来自蜂箱的温度数据，并将所有数据发送到 Apitronics 蜂箱。[Ken]还会将其传输到云服务，这样他就可以实时监控他们。[Ken]希望看到尽可能多的数据，并为美国宇航局的[蜜蜂网](http://honeybeenet.gsfc.nasa.gov/)项目做出贡献，因此他建立了第二个蜜蜂单位来处理附近的 Apitronics 气象站。

![SpaceWrencher](img/4892437613088ab3882681a2ec04a2bb.png) **本帖介绍的项目是[入围 Hackaday 奖的半决赛。](http://hackaday.io/list/2864-The-Hackaday-Prize%3A-Semifinalists)**