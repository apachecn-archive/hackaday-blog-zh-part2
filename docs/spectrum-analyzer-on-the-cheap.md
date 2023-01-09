# 便宜的频谱分析仪

> 原文：<https://hackaday.com/2015/03/12/spectrum-analyzer-on-the-cheap/>

如果你有一台兼容 NTSC 制式的电视，你可以自己造一台真正便宜的频谱分析仪。从那里开始，你只需要一个小硬件来完成这个构建。[Bruce Land]已经推出了一款[频谱分析仪，价格应该不会超过 5 美元](http://hackaday.io/project/4592-pic32-spectrum-analyser)，如果这就是让你不把这个工具添加到你的工作台中的原因的话！

频谱分析仪基于 PIC32 微控制器，该微控制器之前已经在他的示波器项目中得到验证。[布鲁斯]已经设法从这个坚固的芯片中挤出了相当多的东西；频谱分析仪具有 450 kHz 带宽，运行 256 Hz 电视显示器，每秒可输出超过 30 次更新。微控制器运行快速傅立叶变换(FFT)进行计算，结果非常好。

[Bruce]注意到该项目基于另一个项目的电视框架，并在此基础上添加了 FFT。如果你一直在寻找廉价的频谱分析仪，请务必在项目网站上查看源代码，如果你需要处理能力更强但价格稍高的东西，请查看运行在 Raspberry Pi 的 GPU 上的 [FFT。](http://hackaday.com/2014/01/31/fft-on-the-raspis-gpu/)