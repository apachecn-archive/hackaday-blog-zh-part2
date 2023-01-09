# 使用 LED 作为简单的射频检测器

> 原文：<https://hackaday.com/2015/04/26/using-an-led-as-a-simple-rf-detector/>

当[b.kainka]着手制造世界上最简单的射频探测器时，他可能没有意识到它会这么容易。仅由少数几个元件和 38 行代码组成，他就能制造出一个相当好用的[射频探测器](https://hackaday.io/project/5390-integrating-rf-led-detector-with-attiny13)。

运行代码的微控制器是一个在[麻雀板上的 ATtiny13。他使用日常 LED 作为检测二极管，并在 ATtiny13 中使用内部上拉电阻作为偏置电压。天线从 LED 的阳极引出。为了让它足够灵敏，他在一小段时间内接通上拉电阻。因为 LED 可以像一个小电容器一样工作，所以它可以充电到几伏。然后，他关闭上拉电阻，LED 两端的电压将开始放电。如果存在射频信号，放电电压将低于无信号时的放电电压。很棒的东西。](https://hackaday.io/project/4926-cheepit-sparrow-dev-boards-for-smartphones)

请务必查看顶部链接的 Hackaday.io 页面，获取完整的源代码、原理图和一些演示他的项目的视频。

[https://www.youtube.com/embed/VrISHXWsJ9I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/VrISHXWsJ9I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)