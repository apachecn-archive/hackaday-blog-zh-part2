# 将 Arduino 放入树莓派的正确方法

> 原文：<https://hackaday.com/2012/07/23/the-proper-way-to-put-an-arduino-in-a-raspberry-pi/>

尽管他们大吹大擂，树莓 Pi 上的 GPIO 引脚本身并不十分有用。当然，您可以输出数字数据，但我们的世界是模拟的，这些神奇的 Raspi 引脚上没有任何 ADC 或 DAC。

由怀奥勒姆·OSHW 合作组织的[凯文]、[阿诺]和[贾斯汀]设计的 AlaMode 项目旨在解决这一问题。他们为 Raspberry Pi 开发了可堆叠的 Arduino 兼容板。

AlaMode 立即直接插入 Raspberry Pi 的 GPIO 引脚。从那里，与 Arduino 的 ATMega 的通信被启用，允许您像使用 Arduino 一样发送和接收数据。有一个实时时钟，伺服头，许多给电路板供电的方法，甚至还有一个突破[这个 GPS 模块](http://www.youtube.com/watch?v=y1I3Gi3X3HU&feature=context-vrec)。

阿拉莫德省去了许多不必要的费用；没有 USB 端口，但可以直接通过 Raspberry Pi 的 GPIO 引脚进行编程。非常漂亮，我们等不及要为我们的 Raspi 抓一个了。