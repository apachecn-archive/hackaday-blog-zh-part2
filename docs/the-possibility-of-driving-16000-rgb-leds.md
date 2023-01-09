# 驱动 16，000 个 RGB LEDs 的可能性

> 原文：<https://hackaday.com/2015/04/16/the-possibility-of-driving-16000-rgb-leds/>

就像我们认识的每个人一样，[Luis]认为建造一个巨大的 RGB LED 矩阵是一件很酷的事情。然而，巨大的 LED 矩阵很难构建:你不仅要处理大功率需求和不可避免的过热问题，还需要驱动一船 LED。这并不容易。

[Luis] [找到了一个解决问题的方法，用一个新的、奇特的 ARM Cortex M4 微控制器来驱动这些 led](https://sites.google.com/site/luiselectronicprojects/projects/rgb-matrix/ws2812-dma-ping-pong-mode)。所有的 Cortex M4 arm 都有 DMA，使自动内存传输到外设和 LED 灯变得轻而易举。

微控制器[Luis]每个传输集仅支持 1024 次传输，相当于每次传输最多 14 个 led。这个问题可以通过在 DMA 控制器中使用乒乓模式来解决，即针对每个 DMA 请求在数据结构之间切换。基本上，他扩展 led 的数量只是在两个内存区域之间切换，并设置 DMA 传输。

结果比[Luis]的原始电路好得多，原始电路只是一堆 SPI 线。从下面的视频来看，它看起来真的很好。这还不是一个巨大的 LED 矩阵，但如果你想看看它会是什么样子，[看看悬挂在 Hackaday 霸王办公室的巨大的 6 乘 4 英尺矩阵](https://hackaday.io/project/3-fled)。

[https://www.youtube.com/embed/7e5a0nB6AfQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/7e5a0nB6AfQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)