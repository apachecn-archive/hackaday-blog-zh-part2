# 简单的 10 瓦 LED 驱动器是热门的东西

> 原文：<https://hackaday.com/2013/11/20/simple-10-watt-led-driver-is-hot-stuff/>

[Peter]需要为他的显微镜驱动高功率 LED。他没有选择商用 LED 驱动器，[而是构建了一个简单的恒流 LED 驱动器和风扇控制](http://www.instructables.com/id/10W-LED-driver-and-dimmer/)。过去，我们曾在 Hackaday 上介绍过[【彼得】的南瓜蜡烛 LED](http://hackaday.com/2013/10/01/leds-turn-the-heat-up-on-flameless-pumpkin-lights/) 作品。今天，他转向更高功率的 led。对于旧的卤素/光纤环形灯装置，10 瓦的 LED 将是一个很好的替代光源。[Peter]从他的旧备用设备开始-一个 8 针微芯片图片。在这种情况下，PIC12F1501。一张 PIC 不能单独处理 10 瓦的 LED，所以他利用了 Semi 的 [CAT4101 恒流 LED 驱动器](http://www.onsemi.com/PowerSolutions/product.do?id=CAT4101)。PIC 在该电路中执行三项任务。它处理来自两个按钮的用户输入，为 LED 驱动器生成 PWM 信号，并为冷却风扇生成 PWM 信号。

控制很简单:按下两个按钮，LED 灯就会完全亮起。按下“向上”按钮，LED 可分 10 步从 10%升至 100%。“向下”按钮会降低 LED 电源。[彼得]甚至有一个备用的别针。他目前正将其用作 LED 开/关确认，尽管我们可能会将其与 1 线温度传感器一起使用，作为 CAT4101 内置热保护的备份。这可能有点过了，但我们也会将按钮从 7805 线性调节器上移开。由于这种电路将与显微镜一起使用，它最终可能仅通过触摸来操作。如果你试着按下一个按钮，结果却是一个烧焦的指尖，那就有点令人惊讶了！

[https://www.youtube.com/embed/2g89JlYU1RA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/2g89JlYU1RA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)