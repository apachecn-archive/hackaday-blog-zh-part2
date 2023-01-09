# ATMega1284P 原型制作

> 原文：<https://hackaday.com/2015/01/02/prototyping-with-the-atmega1284p/>

当大多数人转向 arm 和其他高规格微控制器时，[戴夫·切尼]却在逆势而为。不要担心，这是一个很好的理由——他正在继续研究那些老式 CPU/微控制器混搭中的一个，它在两个芯片中实现了整个老式系统。

在研究这个项目时，他发现他正在使用的微控制器 ATMega1284p 实际上非常酷。它的内存是广受欢迎的 328p 的八倍，是 Arduino Mega 中 ATMega2560p 的两倍。128k 的闪存，4k 的 EEPROM，32 个 io 和 8 个模拟输入，它真的开始看起来像 Arduino *应该围绕*构建的芯片。当然，历史选择并不重要，因为【戴夫】[可以自己制作 1284p 原型板](http://dave.cheney.net/2014/12/31/building-an-atmega1284p-prototype)。

电路板采用熔结布局，只有几个部件，包括一个晶体、几个电容、一个 ISP 连接器和一个串行连接器引脚。不多，但这就是你需要的原型板。

bootloader 由[Maniacbug]的 [Mighty 1284 Arduino 支持包](http://maniacbug.wordpress.com/2011/11/27/arduino-on-atmega1284p-4/)处理。这仅支持 Arduino 1.0，不支持更新的 1.5 版本，但现在[Dave]有了一个很棒的小原型板，可以在几个小时内将 perfboard 和裸组件组装在一起。这也是继续开发[【戴夫】的 Apple I 复制品](http://hackaday.com/2014/12/26/weird-clocks-and-a-three-chip-apple-i/)的一个很好的工具。