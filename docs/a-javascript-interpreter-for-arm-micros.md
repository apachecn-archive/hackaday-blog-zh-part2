# ARM 微处理器的 JavaScript 解释器

> 原文：<https://hackaday.com/2012/10/05/a-javascript-interpreter-for-arm-micros/>

![](img/fa8b841966cc41ef1d742007cce1900c.png "js")

当编程一个微控制器来执行你的命令时，你只有两个选择。你可以用适当的语言编写代码，比如 C 语言，并把你的源代码交叉编译成一个微处理器容易理解的固件。或者，您可以在微控制器上加载一个解释器，并通过串行连接编写代码。解释器是深入了解硬件的一种非常快速简单的方法，但不幸的是，大多数可用的微控制器解释器都是基于 BASIC 或 Forth 的。

[Gordon]认为现在已经不是 1980 年了，这些相对低级语言的解释器不太适合今天的微控制器。为了解决这个问题，[他创建了 Espruino](http://www.pur3.co.uk/espruino/) ，这是一个用于新一批 ARM 开发板的 JavaScript 解释器。

Espruino 是为 STM 32 VL Discovery board 设计的，尽管[Gordon]计划将他的解释器移植到 Arduino 上，只要他能得到一个解释器。安装就像上传任何其他固件一样简单，即使[Gordon]的 STM32VL 没有串行终端的 USB 端口，连接 USB 到 TTL 转换器并让这个解释器工作也很容易。

Espruino 还没有开源*，*仅仅是因为【Gordon】想要清理他的代码并写一些文档。他还想让 Espruino 盈利，这样他就可以全职从事这项工作，所以如果有人知道(戈登)如何做到这一点，请在评论中留言。