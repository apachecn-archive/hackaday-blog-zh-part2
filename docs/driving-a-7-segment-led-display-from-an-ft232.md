# 从 FT232 驱动 7 段 LED 显示屏

> 原文：<https://hackaday.com/2015/08/29/driving-a-7-segment-led-display-from-an-ft232/>

有时候，一个好的技巧是少用而不是多用。来自[Rahul]的这篇整洁的教程就是如此。S]使用 FT232 驱动 [7 段 LED 显示屏。通过使用这种廉价的 USB 转串行控制器，[Rahul。S]能够在不使用微控制器的情况下直接驱动显示器，从而降低了元件成本。](http://xanthium.in/interfacing-7-segment-led-display-with-ft232-and-d2xx-library)

他正在[位敲打](http://hackaday.com/2009/09/22/introduction-to-ftdi-bitbang-mode/)一个连接到显示器的八进制缓冲器。您可能会惊讶地发现，FT232 芯片确实有足够的输出来实现这一点。不是将串行数据发送到显示器并让控制器将其转换成一组构成数字的信号，这种转换是由 PC 完成的，然后 PC 发送一个信号直接点亮 LED 的适当部分。通过使用 FT232 的所有可用输出线路(包括通常用于信号传输的 RTS/CTS 线路)，[Rahul。S]能够驱动所有七个元素和小数点。

当然，愤世嫉俗者可能会争辩说，使用[廉价的串行 LCD 显示器](http://www.adafruit.com/products/784)会更简单。这是真的，但是知道如何自己做一件事而不是让别人替你做这件事总是有道理的……

[https://www.youtube.com/embed/SaTPUVlcq1g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/SaTPUVlcq1g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)