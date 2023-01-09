# 降压(和升压)转换器初级读本

> 原文：<https://hackaday.com/2015/01/24/a-primer-on-buck-and-boost-converters/>

我们都知道电气系统使用交流电的原因是因为使用变压器可以很容易地将电压升高或降低，这是 DC 系统无法实现的功能……难道不是吗？也许你以前听说过神秘的 DC-DC 变形金刚，但从来没有真正想看看使它们成为可能的魔法。现在，SparkFun 工程总监[Pete Dokter]有一个[教程，解释这些神秘设备如何工作](https://www.youtube.com/watch?v=yf9F3nqZH_Y)。

如果降压转换器降低输入电压，则称为降压转换器；如果升压转换器升高输入电压，则称为升压转换器，[Pete]解释了这些电路如何利用电感的特性来抵抗电流的变化。他非常详细地解释了晶体管或 MOSFETs 等元件如何用于快速切换流向电感的电流，以及磁场发生了什么变化，使得这些器件成为可能。

如果你一直想更好地了解这些设备，视频提供了大量的背景知识。也有一些项目利用这些设备，例如一个使用 [AVR 微控制器来执行小电路](http://hackaday.com/2009/07/07/avr-boost-converter/)的开关，或者另一个使用这些电路的有趣属性来[跟随太阳能电池板的 I-V 曲线](http://hackaday.com/2014/05/05/boost-peak-power-tracking-battery-charger/)来帮助给一组电池充电。可能性是无限的！

[https://www.youtube.com/embed/yf9F3nqZH_Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/yf9F3nqZH_Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)