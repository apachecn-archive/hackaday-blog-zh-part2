# 用微控制器读取 N64 控制器

> 原文：<https://hackaday.com/2012/10/16/reading-an-n64-controller-with-a-microcontroller/>

![](img/c172a3942ef05bba605248a4c92e4701.png "N64")

我们已经看到了 NES、SNES、世嘉，以及雅达利推出的几乎所有与微控制器相连的怪异控制器，但将 N64 控制器连接到一个项目仍然是那些很少见到、很少被复制的努力之一，全球各地的制造商并不经常解决这个问题。[Pieter-Jan]决定参加比赛，尝试用 PIC 读取 N64 控制器，我们很高兴地报告他已经完全成功了。

阅读 N64 控制器的困难之一就是速度；由于控制器端口上只有三个引脚，N64 控制器使用串行协议以相当快的速度发送 32 位控制器数据。有了 PIC18F 'micro 之后，[Pieter]意识到用 C 编程会太慢，他需要一路走到裸机，用汇编语言编写他的 micro。

每次需要读取 N64 控制器数据时，控制台都会发出一个 9 位轮询请求。控制器依次以 32 位序列响应，通知控制台所有按钮和操纵杆的状态。一旦[Pieter]让他的微处理器发送正确的轮询响应，就只剩下解析从控制器返回的数据的问题了。

现在，[Pieter]有一个小型演示板，每当按下 A、B 或 Z 按钮时，LED 就会闪烁。这可以扩展到其余的按钮和操纵杆，但现在我们将在休息后欣赏[Pieter]的演示。

[https://www.youtube.com/embed/AbpkrEaDG2Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/AbpkrEaDG2Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)