# 真正专业的 Raspi 模拟输入

> 原文：<https://hackaday.com/2012/09/14/a-truly-professional-raspi-analog-input/>

令硬件修补者懊恼的是，Raspberry Pi 的 GPIO 引脚上没有模拟输入。当然，你只需要几个控制台命令就可以让 LED 闪烁，但是用骨锉读取传感器需要一点额外的硬件。[Brian Dorey]刚刚发布了一个板，它允许在树莓 Pi 上有 8 个模拟输入，分辨率为 16 位，远高于任何基于 Arduino 的构建。

[Brian]的构建基于去年 7 月我们看到的 Raspi 模拟板的早期类似版本。像以前的版本一样，新的专业制造的 PCB 使用一对微芯片 MCP3428 模数转换器。这些 ADC 能够以 16 位的分辨率对四个通道进行采样；与每个 Arduino 上的 8 位 ADC 相比，这是一个巨大的改进。

这些板通过 I2C 串行总线，使用简洁的可堆叠接头与 Raspberry Pi 通信。理论上，应该可以使用几个这样的板来测量几十个模拟通道，但我们将把演示留给[Brian]。