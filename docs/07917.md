# 和巴士海盗一起学习 I2C

> 原文：<https://hackaday.com/2014/12/27/learning-i2c-with-the-bus-pirate/>

当一个空气质量显示项目需要一个显示器时，[Inderpreet]研究了基于字符的小型液晶显示器。[inder preet]选择的 LCD 使用了 I2C 接口，这对他来说是新的。与其躲避，不如抓住他的巴士海盗，一头扎了进去！

[I2C 或内部集成电路](http://en.wikipedia.org/wiki/I%C2%B2C)串行接口在黑客日经常被提到。它们通常很容易使用，但是和所有的东西一样，有一些小问题会让你第一次旅行的时候更加颠簸。其中之一是电压接口——I2C 使用双向开漏线路，因此与 3.3 V 和 5V 电路接口需要一个电压电平转换器电路来满足这一要求。幸运的是，在[inder preet]的案例中，他的 TI launchpad target devboard 和 LCD 都使用 3.3 伏逻辑电平。

在使用 TI 之前，[Inderpreet]想先测试一下总线盗版。这将允许他验证硬件，并确保他正确地使用 I2C 总线。总线盗版可以在 3.3V 或 5V 逻辑电平下运行，并且具有针对 I2C 总线的板上编程。控制总线盗版就像连接一个串行终端程序并插入 USB 电缆一样简单。

I2C 总线协议相对简单，但是对于一个新用户来说仍然是混乱的。在数据字节开始流动之前，每个事务都需要一个地址、读/写位和一个按正确顺序发送的启动命令。还有确认位，证明数据字节确实被 LCD 接收到。“巴士海盗”让这一切变得简单，让[Inderpreet]在他的 LCD 模块上快速显示“你好”。

I2C 巴士只是巴士海盗的冰山一角。如果您有兴趣了解更多信息，请访问[hack aday 商店查看！](http://store.hackaday.com/products/buspirate-v3-6-thm180c4m)

[via [危险原型](http://dangerousprototypes.com/2014/12/26/getting-started-with-an-i2c-lcd-using-a-bus-pirate/)