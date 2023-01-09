# 利用 DMA 驱动 WS2812 LED 像素

> 原文：<https://hackaday.com/2013/11/22/using-dma-to-drive-ws2812-led-pixels/>

众所周知，LED 像素硬件开始变得普遍，WS2811 和 WS2812 都需要非常严格的时序来解决这些问题。那里有一些库，这意味着你几乎不需要做任何工作，但是这一点也不好玩。[Elia]开始研究驱动硬件需要什么，在 STM32VL 发现板的帮助下，在转向 32 位之前尝试了一些 8 位微处理器。转向更强大的处理器带来了更快的速度，但是为什么要对所有的东西都进行位爆炸呢？他想出了一个办法[利用芯片的 PWM 和 DMA 特性来驱动 led](http://eliaselectronics.com/driving-a-ws2812-rgb-led-with-an-stm32/)。

DMA 是直接内存访问单元，允许您在不中断处理器的情况下更改发送到像素的值。这是通过在存储器位置预加载数据来完成的。该缓冲区由 DMA 单元自动读取，其值用于设置 PWM 定时器比较触发器，以便发送上图所示的逻辑值。

如果你想更深入地研究这个话题，这里有一组驱动 WS2811 的[技术。](http://hackaday.com/2013/01/02/three-conceptual-approaches-to-driving-a-ws2811-led-pixel/)

[https://www.youtube.com/embed/EZa9yF68Im8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/EZa9yF68Im8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)