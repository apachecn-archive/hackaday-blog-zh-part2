# 来自微处理器时钟输出的莫尔斯码射频发射机

> 原文：<https://hackaday.com/2015/02/16/morse-code-rf-transmitter-from-a-micros-clock-output/>

如果你正在寻找一种简单的方法来制作射频发射器，看看[托马斯]的莫尔斯电码发射器。他的设计只使用了一个微控制器和一个 16 兆赫的晶体来传输 96 兆赫的连续波莫尔斯电码。我们已经看到一些[类似的设计，工作在较低的频率](http://hackaday.com/2010/07/27/200-mile-rf-transmitter-and-high-altitude-balloon/)，但传输高达 96MHz 是非常令人印象深刻的。

[Tomasz]在这个项目中使用了一个 STM32L 微控制器，该微控制器不能在他想要传输的高频下运行。为了解决这个问题，[Tomasz]在微控制器的时钟输入端连接了一个 16Mhz 的振荡器。时钟输入进入能够产生高频的微处理器 PLL。他提到可以使用内部振荡器来代替晶体，但它有大量的相位噪声，会分散到整个频谱中。

[Tomasz]选择以 96MHz 开始传输，这可以通过标准的 FM 无线电接收。为了产生该频率，他设置 PLL 将 16MHz 晶振倍频至 192MHz，然后进行 2 分频，使其降至 96MHz。微控制器的 CPU 在 16MHz 晶振输入进入 PLL 之前运行。接下来[Tomasz]启用 MCO 时钟输出引脚，将 96MHz 信号发送到外部世界。

传输 CW 非常简单；它只需要打开和关闭一个固定频率的发射机。[Tomasz]写了一个函数来启用和禁用 MCO 输出引脚。这具有键入你扔给它的任何莫尔斯电码串的效果。休息后，请观看视频，了解发射机的工作情况。

[https://www.youtube.com/embed/nZnpINK2aoI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/nZnpINK2aoI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)