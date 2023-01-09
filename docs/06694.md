# PS/2 Synth 会让你大吃一惊

> 原文：<https://hackaday.com/2014/07/31/ps2-synth-will-knock-you-off-your-broom/>

这里有一个围绕着很多人都有的东西的黑客:一个 PS/2 键盘。[serdef]将一台[哈利波特版 PS/2 变成了一台 synth 键盘和鼓机的组合](http://hackaday.io/project/2148)，并在 Hackaday.io 上有一篇关于它的很好的报道。

为了通信，他撕掉了一根 PS/2 转 USB 电缆，得到一个女性迷你 DIN 连接器，并将其连接到 Nano。他使用 Dreamblaster S1 合成模块来产生声音，这个模块和 Nano 一起放在合成屏蔽上。合成器可以由 USB 或 9 伏电源供电。

键盘映射是通过 Teensy PS/2 键盘库完成的。[serdef]重用了来自他的自行车鼓手项目的大量代码，该项目也使用了 Dreamblaster S1。[serdef]正在为这个项目不断添加功能，就像一个谐振控制锅，让他像模拟合成器一样塑造波形。他发布了一些方便的 PS/2 集成代码、他的 synth 代码和一个 KiCad 原理图。演示视频在链接对面等着你。

作为鼓机:

[https://www.youtube.com/embed/-dhS0qbpMqM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/-dhS0qbpMqM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

作为一个甜美的合成器:

[https://www.youtube.com/embed/tHh1QaiP8c8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/tHh1QaiP8c8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)