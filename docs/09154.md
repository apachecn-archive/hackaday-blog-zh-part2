# 使用 3D 打印的注射泵架提升容量

> 原文：<https://hackaday.com/2015/05/29/pump-up-the-volume-with-the-3d-printed-syringe-pump-rack/>

当必须以一定的速率和体积分配特定量的流体时，注射泵是有价值的工具。它们有多种用途，用于通过液相色谱(LC/HPLC)进行静脉给药。不幸的是，一个商业泵可以花费一大笔钱。对高昂的价格并不特别兴奋，[Aldric Negrier]卷起袖子，以 300 美元制作了一个 3D 打印版本。

在之前 [Hackaday 上已经出现过【Aldric】，所以我们知道他的最新项目不会让人失望。他的 3D 打印注射泵架包含五个独立的泵，可以彼此独立运行。每台泵的外壳由五块 3D 打印而成。此外，每个泵都由一个特氟隆涂层丝杠、一个 Arduino Nano V3、一个 Pololu 微型步进电机驱动器和一个 NEMA-17 步进电机组成。3D 打印的注射泵架在 12V 电源下运行，每个电机最大使用 2 安培。](http://hackaday.com/2015/03/22/take-a-spin-on-this-voice-controlled-3d-scanning-rig/)

虽然标准的 Arduino IDE 包含步进器库，但[Aldric]想要一个允许更精确控制的库，于是就有了 [Accelstepper](http://www.airspayce.com/mikem/arduino/AccelStepper/) 库。3D 打印的注射泵架，10ml 的注射器，测量精度 0.5 l，没什么好嘲笑的。

像[Aldric's]这样的注射泵架是另一个很好的例子，它使用开源资源和 DIY 精神，使通常昂贵的技术对较小的实验室来说更加经济实惠。如果你对其他开源注射泵设计感兴趣，你可以看看这个 2014 年[黑客日奖](https://hackaday.io/project/1838-open-syringe-pump)的参赛作品。

[https://www.youtube.com/embed/0qY2Ud9Oslo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/0qY2Ud9Oslo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)