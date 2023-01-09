# 最小的 WS2812B 驱动程序

> 原文：<https://hackaday.com/2014/12/17/the-most-minimal-ws2812b-driver/>

无论你称它们为单独可控的 RGB LEDs、WS2812 还是 NeoPixels，不可否认它们非常受欢迎，是每个 glowey 和 blinkey 项目的主要内容。刚从卷轴上取下时，它们几乎没有用——你需要一个控制器，这导致许多人对同一个问题提出许多不同的解决方案。[这是另一个解决方案](http://jeelabs.org/book/1450d/)，值得注意的是它是我们见过的最小的 WS2812 驱动程序。

这一构建中的关键组件是[恩智浦的 LPC810](http://www.nxp.com/products/microcontrollers/cortex_m0_m0/lpc800/LPC810M021FN8.html) ，一款采用 8 引脚 DIP 封装的 ARM Cortex M0+。是的，它是 DIP-8 中唯一的手臂，但仍然能够以 30MHz 的速度运行，并保存 4kB 的程序。

JeeLabs 使用 LPC810 上的 SPI 总线以 led 所需的速率输出数据。唯一需要的硬件是一个将电压从 5V 降至 3.3V 的小型 LED 和一个去耦电容。是的，作为一个单一组件的构建，您可以很容易地摆脱它。

构建由 60 个 WS2812b RGB LEDs 组成，芯片尽职尽责地以正确的速率输出位。这是一个 LED 时钟项目的完美开端，一个钢铁侠电弧反应堆(我们还在做那些吗？)，或者只是塞进可穿戴设备中的随机闪烁发光二极管。

谢谢[马丁]送来这封信。