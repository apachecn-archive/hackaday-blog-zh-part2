# 阿蒂尼升压转换器

> 原文：<https://hackaday.com/2014/12/07/an-attiny-boost-converter/>

这个原理图是你构建自己的电压转换器所需要的。[Lutz]需要一个可以将 5 V 提升到 30 V 的转换器，为一串 led 供电。解决方案是使用低成本 ATtiny85 和一些无源元件[实现升压转换器](http://www.hackerspace-ffm.de/wiki/index.php?title=LED_step-up_converter_with_ATtiny85)。

该电路遵循经典的[升压转换器](http://en.wikipedia.org/wiki/Boost_converter)拓扑结构，使用 ATtiny85 控制开关。10 欧姆电阻反馈到微控制器的 ADC 输入端，使其能够检测输出电压。通过测量输出电压并相应地调整占空比，电路可以调节到指定的电压设定点。

电位计用于改变发光二极管的亮度。软件读取电位计的输出电压，并相应地调整电路的电压输出。电压越高，led 越亮。

当然，还有许多其他方法来实现升压转换器。大多数实际设计将使用为此特定目的设计的芯片。但是，如果您对开发自己的产品感兴趣，可以使用源代码和 LTSpice 仿真文件。