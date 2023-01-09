# 这个模拟机器人在边线外比赛

> 原文：<https://hackaday.com/2014/10/18/this-analog-cambot-plays-outside-the-lines/>

跟线机器人的味道还真不少。不管它们是如何制造的，大多数都是为了速度和准确性而制造的。然而，Jorge Fernandez 的 Cambot 利用传统的摄像机来读取视觉输入，而不是我们在这些类型的机器人中常见的反射传感器。正因为如此，它缺乏那些迅速和敏捷的品质，但凭借其独特的模拟设计，超大的三轮车车轮和侧面突出的时尚 RCA 插孔得分。

加上 PIC 16F84A 微控制器，[Fernandez]将摄像机的视频输入分成 625 行。PIC 负责水平扫描这些线，并将黑白比例转换成 PWM 脉冲。摄像机观察到这些比例的持续时间决定了供给驱动机器人的左右伺服电机的 PWM 频率。

至于线追随者去，这是一个令人耳目一新的复古的概念。[埃尔南德斯]在他的博客上概述了驾驶他的 [cambot](http://www.zonabot.com/19-cambot-micro-robot-sigue-lineas-con-camara-de-tv.html) 的技巧(英文翻译可以在这里阅读)，并为那些对制造自己的古怪小机器感兴趣的人提供了完整的示意图。

[https://www.youtube.com/embed/-Bl7kCK2H44?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/-Bl7kCK2H44?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)