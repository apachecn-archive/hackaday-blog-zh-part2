# 逆向工程蜡烛闪烁发光二极管

> 原文：<https://hackaday.com/2013/12/16/reverse-engineering-a-candle-flicker-led/>

蜡烛闪烁发光二极管是一个真正的蜡烛一部分的替代品。它们包含一个黄色 LED 和一个控制芯片，可以调节光线以产生蜡烛效果。[Cpldcpu]深入研究了其中一个 led 的逆向工程[。](http://cpldcpu.wordpress.com/2013/12/08/hacking-a-candleflicker-led/ "Hacking a Candleflicker LED")

为了分析封装在 LED 本身中的电路，将一个分流检测电阻连接到 LED。通过将该电阻连接到逻辑分析仪，可以观察到控制信号。

这个控制信号看起来像脉冲宽度调制，占空比有一些随机性。[Cpldcpu]确定一个[线性反馈移位寄存器](http://en.wikipedia.org/wiki/Linear_feedback_shift_register)最有可能用于产生一个 pseudeorandom 比特流，并应用一些整形使 LED 看起来更像一个真正的蜡烛。

事实证明，闪烁的 LED 可能相当复杂，这需要通过分析信号来深入了解它。[Cpldcpu]吸取经验教训，为 AVR 编写了算法的[实现。](https://github.com/cpldcpu/CandleLEDhack)