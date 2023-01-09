# TFT 液晶显示器以 Teensy 3.1 的速度达到了极限

> 原文：<https://hackaday.com/2014/08/18/tft-lcds-hit-warp-speed-with-teensy-3-1/>

被称为 Teensy 之父的[Paul Stoffregen]利用 Teensy 3.1 的硬件，通过 SPI 驱动的 TFT LCD 获得了一些重大的速度提升。如今，低成本串行 TFT LCDs 已经变得很普遍。我们很多人都使用 [Adafruit 的 TFT LCD 库](https://github.com/adafruit/TFTLCD-Library)来驱动 Arduino 上的这些显示器。Adafruit 库为我们提供了一个简单的 API 来处理这些 LCD，使我们不必学习各种复杂的驱动芯片。

[Paul]通过使用 Teensy 3.1 的 32 Freescale Kinetis K20 微控制器上可用的硬件来增强该库。第一个障碍是原始速度。Arduino 的 ATmega328 可以以 8MHz 的速度驱动 SPI 总线，而 Teensy 的 Kinetis 可以将速度提高到 24MHz。

然而速度并不是一切。[Paul]还使用飞思卡尔的 4 级 FIFO 来缓冲传输。通过使用“先写入，然后阻塞，直到 FIFO 未满”算法，[Paul]确保新数据总是尽快到达 LCD。

另一个巨大的进步是 SPI 芯片选择。Kinetis 可以从硬件驱动多达 5 个 SPI 片选引脚。ATmega328 不支持芯片选择。因此，它们必须用 GPIO 引脚来实现，这需要更多的时间。

最后的结果相当令人印象深刻。点击休息时间观看基于 ATmega 的 Arduno 与 Kinetis K20 驱动的 Teensy 3.1 的比赛。

Paul 的图书馆是开源的，可以在 Github 上获得。

[https://www.youtube.com/embed/tioOB3Ysz70?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/tioOB3Ysz70?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

**更新:**为了回应评论中的一些问题，【Paul】添加了第二个视频，比较 Teensy 3.1 和 Arduino Due。Due 以更高的 SPI 时钟速度运行，然而 Teensy 凭借其硬件优势和优化的库仍然被证明更快。

[https://www.youtube.com/embed/rL_2_D3cgFg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/rL_2_D3cgFg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)