# 利用基于 DMA 的 SPI 驱动 WS2812B 像素

> 原文：<https://hackaday.com/2014/09/10/driving-ws2812b-pixels-with-dma-based-spi/>

驱动 ws 2812 b(ws 2811)RGB led 的常用方法通常是对 I/O 线进行位碰撞。然而，这占用了宝贵的微控制器周期，同时等待翻转一点。一种占用处理器资源较少的方法是使用内置串行外设接口(SPI)模块。这是通过特制的数据和波特率设置来实现的，当通过串行数据输出(SDO)引脚移出时，会重新创建所需的 WS2812B 信号时序。即使在 SPI 模式下运行，您的硬件 TX 缓冲区大小也会限制在没有 CPU 干预的情况下可以更新的像素数量。

[Henrik]通过对微芯片 PIC32MX250F128B 微控制器中的 SPI 模块使用[外设 DMA(直接存储器访问)来绕过这一限制。正确配置后，DMA 控制器将自动递增 DMA RAM 的定义部分，将像素数据发送到 SPI 模块。由于 DMA 控制器负责传输，所以微处理器可以自由地做其他事情。这使得所有的 DMA 内存成为你的显示缓冲区。并留下大量宝贵的微控制器周期来计算您希望 RGB LEDs 显示什么模式。](http://blog.gitmi.com/interfacing-ws2812b-ws2811-rgb-leds-with-a-pic32mx-250f128b-micro-controller-spi-700-khz-update-3/)

上面的链接提供了源代码，供那些想仔细阅读或尝试的人使用。这是【亨里克】[像素艺术项目](http://blog.gitmi.com/pixel_art_project/)的一部分。中断后基于 DMA 的 SPI 像素视频:

[https://www.youtube.com/embed/E2cM_xwJCP4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/E2cM_xwJCP4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

欲了解更多基于 DMA 的 WS2812B 像素，请查看基于此 [PWM 的版本](http://hackaday.com/2013/11/22/using-dma-to-drive-ws2812-led-pixels/)。