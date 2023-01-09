# 它继续前进… Arduino 版

> 原文：<https://hackaday.com/2015/07/24/it-keeps-on-going-and-arduino-edition/>

三节 AA 电池能让一个 Arduino 电路运行多久？经过精心设计，[educ8s]制造了一个[温度传感器](http://educ8s.com/Arduino/DS18B20/)，它可以在三个 2250 mAH 可充电电池充电一次的情况下持续使用一年多(或者至少应该持续这么长时间)。

像大多数长寿命设计一样，这种温度传感器大部分时间都在休眠。该设计使用了一个 [DS18B20](http://hackaday.com/2015/06/11/arduino-controlled-air-conditioner/) 温度传感器和一个诺基亚 5110 液晶显示器。它还使用光敏电阻在黑暗中关闭液晶显示器，以进一步节能。

在睡眠期间，显示器打开时，器件仅消耗 260 微安电流，显示器关闭时，仅消耗 70 微安电流。每两分钟，处理器唤醒并读取温度，在非常短的时间内消耗大约 12 毫安。

除了代码，[educ8s]还有一个电子表格，它根据不同的测量参数和电池供应商声称的自放电率来计算电池寿命。

当然，有了更大的电池组，你可以通过充电获得更多的服务。如果你需要复习电池选择，我们在不久前的中提到过。或者，如果你想改善你的电池选择，你可以查看一个[荒谬地完成电池比较网站](http://hackaday.com/2014/09/05/an-obsessively-thorough-battery-and-more-showdown/)。

[https://www.youtube.com/embed/TEr-oraSjN0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/TEr-oraSjN0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)