# Arduino Zero Pro 软发布？

> 原文：<https://hackaday.com/2015/03/04/arduino-zero-pro-soft-release/>

Arduino Zero 有一个更新的产品页面，现在被称为[Arduino Zero Pro](http://www.arduino.org/products/arduino-zero-pro)，在 Arduino.org，两个决斗“Arduino”之一。

我们在 2014 年 5 月第一次[报道了 Arduino Zero，此后不久甚至亲眼看到了一个](http://hackaday.com/2014/05/15/introducing-the-arduino-zero/)[开发原型](http://hackaday.com/2014/05/21/arduino-zero-hardware-is-not-just-for-beginners/)。基于 Atmel 的 ARM Cortex-M0+芯片，它建立在比 AVR Arduini 更快的处理器上，并包括 Atmel 的嵌入式调试器，用作 USB 到串行通道和片上调试外设。但到目前为止，我们只看到了原型。

现在，有 2015 年 1 月 7 日的图表和 Eagle 文件。Arduino.org 网站称 Zero Pro“现已上市！”但是在我们最喜欢的在线电子产品经销商那里，我们还看不到任何现货。也许我们找错了地方(不太可能)，或者只是时间问题。

无论如何，在我们随意翻阅新的 Zero Pro 信息时，有两件事让我们印象深刻。

首先，与原型版本的[(图片)相比，有更多更大的去耦电容遍布电路板，从电源到嵌入式调试器芯片，再到缓冲模拟参考电压电平的 4.7uF 钽电容。这表明已经进行了一些真实世界的测试，并对原型的一些设计缺陷进行了测试。这一切都很好，我们希望这是它真的很快上市的标志。](http://arduino.cc/en/uploads/Main/Arduino_Zero_front.png)

其次，考虑到正在进行的商标纠纷，即使是 Zero Pro 原理图的注释也变得很有趣。在打开 [PDF 原理图](http://download.arduino.org/products/ZEROPRO/Arduino-Zero-Pro-V3-SCH.pdf)(自然是 PDF)或任何 Eagle 文件时，通常会出现“不要用这些信息完成设计”的样板文件。但以前的标题是“Arduino 是注册商标”。ARDUINO 名称的使用必须符合 http://www.arduino.cc/en/Main/Policy 的”它现在写道:

**“Arduino”名称和标志是 Arduino S.r.l .在意大利、欧盟和世界其他国家注册的商标。**

(在注意到这一变化后，我们回去比较了 arduino.cc 上的[“rev3”Uno 原理图 PDF 和 arduino.org](http://arduino.cc/en/uploads/Main/Arduino_Uno_Rev3-schematic.pdf)上的[“rev3E”原理图。是的，法律声明也有同样的变化。)](http://download.arduino.org/products/UNO/Arduino-UNO-Rev3e-SCH.pdf)

我们不是律师，但在声明中明显遗漏的“世界其他国家”之一是 Arduino LLC 可能持有商标的美国。我们仍在试图弄清楚这一切，但看到法律之战在 Eagle schematics 的注释中上演很有趣，不是吗？

请继续关注 Arduino vs Arduino 法律战的更多报道，当然，还有新硬件发布后的评论。

感谢[Marc]提供的关于新主板发布的提示。