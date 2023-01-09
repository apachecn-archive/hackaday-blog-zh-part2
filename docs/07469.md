# 使用带有任何 HDMI 接口的手机屏幕

> 原文：<https://hackaday.com/2014/11/02/using-cell-phone-screens-with-any-hdmi-interface/>

由于智能手机在全球的普及，微型高分辨率显示器变得普遍而廉价。除了手机之外，将这些显示器与任何东西连接都是一个问题。[twl] [有一个板就是这样做的](http://hackaday.io/project/364-mipi-dsi-display-shieldhdmi-adapter)，将 HDMI 转换成这些显示器可以理解的东西，并提供一个帧缓冲区，以便这些显示器可以通过小型微控制器写入。

[twl]正在使用一个相当大的 FPGA 来处理从 HDMI 到显示器理解的 DSI 的所有转换。他使用的是 Xilinx Spartan-6-SLX9，这是最受业余爱好者欢迎的设备之一，可以手工焊接。板上还有一点 SDRAM 用于帧缓冲、HDMI 输入，以及 LCD 及其背光的电源。

在[twl]的“待办事项”列表中，将 Doom 移植到手机显示屏上显然是最重要的。他还想测试他的板的 Arduino 侧的绘图命令，允许任何带有后缀~'ino 的板在小型、廉价、高分辨率的显示器上绘制图形和文本。这是两倍于[twl]预计 BOM 的产品所不具备的能力，我们迫不及待地想看看他会拿出什么。

你可以在下面查看[twl]板显示树莓 Pi 输出的演示视频。如果你仔细观察，你会注意到显示适配器的引导/默认屏幕是 Hackaday Jolly Wrencher。

[https://www.youtube.com/embed/vCWGMM00ZEk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/vCWGMM00ZEk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)