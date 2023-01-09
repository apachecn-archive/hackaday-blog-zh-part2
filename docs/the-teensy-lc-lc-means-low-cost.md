# 小小的 LC。LC 意味着低成本。

> 原文：<https://hackaday.com/2015/02/03/the-teensy-lc-lc-means-low-cost/>

出于这样或那样的原因，我们最近已经看到了很多以 Teensy 3.1 为特色的版本。回想起来，这有点显而易见；便宜又快是好板。是的，不知何故[保罗]在好的/便宜的/快速的互斥三人组中击中了所有三个。

现在，有了一个新的少年。这是小小的 LC——低成本。它没有 Teensy 3.1 那么强大，但它确实给了你一只手臂的力量，就像一个带 ATMega 的主板一样便宜。

[Paul]为 Teensy LC 选择的芯片是 [Freescale MKL26Z64](http://www.freescale.com/webapp/sps/site/prod_summary.jsp?code=KL2x&lang_cd=) (数据表[这里](http://cache.freescale.com/files/microcontrollers/doc/data_sheet/KL26P64M48SF5.pdf?fasp=1)和 876 页的参考手册[这里](http://cache.freescale.com/files/microcontrollers/doc/ref_manual/KL26P121M48SF4RM.pdf?fasp=1)。当然是 pdf)。这是一款 32 位 Cortex-M0+处理器，运行频率为 48 MHz，具有 64k 闪存和 8k RAM。它有 27 个数字 I/O 引脚，Teensy LC 设计为与 Teensy 3.0 和 3.1 引脚兼容。

片上有 13 路模拟输入、8 路 PWM 输出、12 位 DAC 输出、3 个串行端口、2 个 SPI 端口和 2 个 I2C 端口。大多数引脚可以驱动 5mA，少数能够驱动 20mA，还有一个 5v 输出引脚用于驱动 WS2812 Neopixel LEDs。

由于这是 Teensy 的精简版，Teensy 3.1 上的所有可用功能都无法放入 Teensy LC 的 BOM 中。引脚不支持 5V，没有 CAN 总线，只有 4 个 DMA 通道，而不是 Teensy 3.1 上的 16 个。尽管如此，它仍然是 ATMega 饰品或其他小型开发板的一个很好的解决方案。