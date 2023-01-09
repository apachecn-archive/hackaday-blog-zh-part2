# Arduino 上的 640×480 VGA

> 原文：<https://hackaday.com/2014/06/10/640x480-vga-on-an-arduino/>

关于 Arduino 生成 VGA 视频输出的接口，即使没有上百个例子，也有几十个。Arduino 不是迄今为止最快的芯片，而且到目前为止，如果你想控制单个像素，所有这些 VGA 生成技术都在较低的分辨率下达到顶峰。【PK】有[一个有趣的技术，在不超频的情况下，以每秒 60 帧的速度生成 640×480 VGA](http://dqydj.net/how-to-produce-640x480-vga-color-video-from-an-arduino/) 。它很粗糙，很丑，但令人惊讶的是，它真的有效。

640×480 @ 60 fps 的 VGA 标准要求像素以 25.175 MHz 输出，Arduinos 中的 ATMega 芯片以 20 MHz 输出。[PK]想要在不超频的情况下产生 VGA 信号，他通过数字逻辑将时钟频率加倍[来实现这一点。ATMega 产生一个时钟，反相器延迟该时钟，使其相位相差 90 度，两个时钟进行异或运算，使微处理器的时钟输出加倍。它在 32 MHz 时产生非常难看的方波，与 VGA 规格相比误差为 27%。不知何故，它仍然有效。](http://dqydj.net/how-to-double-clock-frequency-using-only-digital-logic/)

随着一个滑稽的不合规格的时钟，项目的其余部分从[【尼克·伽马】的 VGA 库](http://www.gammon.com.au/forum/?id=11608)，一个 16×16 的字体集和[一个来自【lft】](http://www.youtube.com/watch?v=sNCqrylNY-0)的项目被拉在一起。下面视频。

[https://www.youtube.com/embed/nmdvhgbsglQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/nmdvhgbsglQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)