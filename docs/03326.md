# WS2811 可以使用 8MHz 时钟以 800kHz 进行寻址

> 原文：<https://hackaday.com/2013/05/27/ws2811-can-be-addressed-at-800khz-using-a-8mhz-clock/>

![ws2811-running-at-8mhz](img/b43751981422fb827b831eea696b390e.png)

时序就是一切，这就是为什么大多数通信协议都需要非常精确的时钟源。WS2811 LED 灯条控制器也不例外。但是[丹尼]想出了一种方法，用 8MHz 时钟源可靠地驱动它们。

WS2811 已成为最受欢迎的 RGB 像素和条带控制器之一。我们已经看到了一些用来解决这些问题的方法，包括[16 MHz AVR 技术](http://hackaday.com/2012/12/07/driving-a-ws2811-rgb-led-pixel/)激发了【Danny】承担这个项目。他计划使用该库，但 16MHz 晶体的 25 天运输时间迫使他发明了一种使用内部振荡器的方法。

黑客的要点是，他编写汇编代码来处理成对的二进制位值。手头有了四种可能组合中每一种的代码块，他必须找到一种方法来精心设计条件跳转，以保持准确的时间。在试图用手解决这个难题碰壁后，他写了一个 C++程序来解决这个问题。证据就在这个视频中，视频显示一个芯片在一条带上驱动多个 Larson 扫描仪。

[https://www.youtube.com/embed/mP7vBw4UeME?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/mP7vBw4UeME?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)