# 高速 SSD1306 库

> 原文：<https://hackaday.com/2015/04/03/high-speed-ssd1306-library/>

[Lewin]来信告诉我们他帮助开发的 Arduino Due 高速库，该库允许与使用 SSD1306 显示控制器的有机发光二极管显示器接口，使用 DMA 例程来加快显示刷新时间。

通常，[单色 1.3 英寸 128×64 有机发光二极管图形显示器](http://www.adafruit.com/product/938)等显示器通过 SPI 或 I2C 总线与 Arduino 板连接。由[Limor Fried]编写的 [Adafruit_SSD1306 库](https://github.com/adafruit/Adafruit_SSD1306)使得使用软件或硬件 SPI 将这些显示器与各种 Arduinos 配合使用变得简单。对于使用硬件 SPI 的标准设置，调用 display()大约需要 2ms。

[Lewin]想让它更快，到期的 SAM3X8E 似乎可以交付。他首先进行了一次搜索，以确定这是否已经完成，但却一无所获。他确实找到了[【马雷克·布里亚克】基于 ILI9341 的 TFT 屏幕库](http://marekburiak.github.io/ILI9341_due/)。[Marek]使用了[William Greiman]的代码，他为 Arduino 开发了 SD 卡库。[William]利用 SAM3X8E 的 DMA 功能实现了更快的 SD 卡传输，然后[Marek]修改了该代码，以允许更快地写入基于 ILI9341 的屏幕。[Lewin]所要做的就是在 Marek 的代码中找到使用 DMA 通过 SPI 发送缓冲区的代码，并将其应用于 SSD1306 的 Adafruit 库。

但是有一个警告:如果您还使用 SPI 与其他硬件接口，使用这个库可能会带来麻烦，因为常规的 SPI.h 库将不再与[Lewin]的库协同工作。他提供了一些如何克服这些问题的技巧，并欢迎任何反馈或测试来帮助改进代码。速度的提高是巨大的。使用标准 SPI 时钟时，速度可提高 4 倍，如果提高 SPI 时钟速度，速度可提高 8 倍。该代码可在他的 Github repo 上获得。