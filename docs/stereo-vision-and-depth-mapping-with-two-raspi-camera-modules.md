# 使用两个 Raspi 相机模块进行立体视觉和深度映射

> 原文：<https://hackaday.com/2014/11/03/stereo-vision-and-depth-mapping-with-two-raspi-camera-modules/>

Raspberry Pi 有一个摄像头连接器端口，允许它捕捉 1080p 视频并将其传输到网络，而不必处理网络摄像头的疯狂和通过 USB 捕捉 1080p 视频的可能性。Raspberry Pi 计算模块稍微高级一些；它打破了*两个*相机连接器，理论上给树莓派立体视觉和深度映射。【大卫·巴克】[把一个计算模块和两个摄像头放在一起](http://www.argondesign.com/case-studies/2014/oct/21/stereo-depth-perception-raspberry-pi/)让这个建筑成为现实。

在计算机视觉和机器人研究中使用立体视觉的时间比其他深度映射方法(如重新设计的 Kinect)要长得多，但迄今为止，实现这一点的硬件有点难以获得。很明显，你需要两台摄像机，但是软件技术在相关的文献中已经很好的理解了。

[David]将两台摄像机连接到一个 Pi 计算模块，并实施了三种不同版本的软件技术:一种是 Python 和 NumPy 版本，运行在 3GHz x86 机器上；一种是 C 版本，运行在 x86 和 Pi 的 ARM 内核上；另一种是汇编语言版本，用于 Pi 上的 VideoCore。在 x86 平台上，Python 可以在 63 秒内完成视差计算，而 C 可以在 56 毫秒内完成。在 Pi 上，C 用了 1 秒，VideoCore 用了 90 毫秒。这相当于 Pi 上大约 12FPS 的帧速率，对于一些非常非常有趣的机器人工作来说绰绰有余。

Raspi 博客上有一些更好的图片，展示了这个设置可以做什么。我们找不到使这成为可能的软件的链接，所以如果有人有链接，请在评论中留下。