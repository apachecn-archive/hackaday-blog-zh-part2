# Arduinos(和其他 AVR)写入自己的闪存

> 原文：<https://hackaday.com/2015/07/03/arduinos-and-other-avrs-write-to-own-flash/>

在 Arduino.cc 论坛上的[这篇文章](http://forum.arduino.cc/index.php?topic=332191.0)和[这篇博客文章](http://majek.mamy.to/en/writing-to-internal-flash-on-arduino/)中，【Majek】宣布他已经欺骗了内部的 AVR 微控制器和 Arduino，在运行时将用户数据写入它自己的闪存。哇！

[Majek]在这里做了一个非常漂亮的黑客攻击。通常，AVR 微控制器不能写入自己的闪存，除非它处于引导模式，当你想保存非易失性数据时，你就只能使用 EEPROM。但是 EEPROM 比较稀缺，相对于 flash 来说。

现在，在正常情况下，写入闪存程序存储器会给你带来麻烦。事实上，AVR 具有保护功能，可以防止未托管在引导加载程序内存块中的代码写入闪存。当然，引导程序必须能够对芯片进行编程，所以肯定有办法进入。

诀窍是[Majek]仔细修改了 Arduino 的 Optiboot 引导程序，使其在已知位置公开一个 flash-write (SPM)命令，这样他就可以从引导程序外部使用该功能。AVR 不会阻止 SPM 继续运行，因为它是从 bootloader 内存中调用的，一切正常。

Optiboot bootloader 的[修改版可以在【Majek】的 Github 上获得。如果你想知道他是如何做到的，](https://github.com/majekw/optiboot)[这里有一些不同之处。特别好的一点是，这些都被包装在易于编写的代码中，带有一个](https://github.com/Optiboot/optiboot/pull/142/files)[工作演示](https://github.com/majekw/optiboot/blob/supermaster/optiboot/examples/flash_program/flash_program.ino)。所以下次你写满了 EEPROM，你就可以用这个工具把你的数据记录到闪存程序中。

感谢[Koepel]的提示！