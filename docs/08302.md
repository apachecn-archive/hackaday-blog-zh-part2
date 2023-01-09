# 近地轨道 MVS 的 HDMI 音频和视频

> 原文：<https://hackaday.com/2015/02/13/hdmi-audio-and-video-for-neo-geo-mvs/>

[Charlie]花了一些时间在他从易贝买的廉价 FPGA 开发板上进行黑客攻击。最初，他打算在有新的灵感之前，用它们来为一个不同的项目创建 HDMI 端口。相反，他给近地轨道 MVS 游戏增加了一个 HDMI 接口。[Neo Geo MVS](http://en.wikipedia.org/wiki/Neo_Geo_%28system%29)是一台 90 年代的街机，玩的是《合金弹头》和《武士对决》系列等游戏。[查理]对 mods 有特殊的诀窍，之前因在硬件上实现[Zork](http://hackaday.com/2014/11/29/the-zork-virtual-machine-implemented-in-hardware/)和制作[迷你 supergun PCB](hackaday.com/2013/11/25/mini-supergun-pcb/) 而在 Hackaday 上亮相。他最新款的特别之处在于，HDMI 可以输出音频和视频。

[Charlie]通过将数字输入接入 Neo Geo 的 DAC(数模转换器)获得了最佳的视频和音频信号。然后使用 FPGA 将信号转换为 HDMI，保持从视频生成到显示的数字信号路径。虽然这听起来很简单，但还有很多事情要做。JAMMA 视频标准的较低分辨率与 HDMI 协议提供的各种分辨率不兼容。[Charlie]通过使用 Cyclone II 开发板上的 RAM 实现扫描加倍解决了这个问题。然后，他必须将音频下采样到 32kHz(从 55.6kHz)，以满足 HDMI 规格。通过 HDMI 获得声音需要在信号中添加数据岛，这是一个令人沮丧的壮举。

当他用他的显示器测试 HDMI 时，它超出了规格，但仍然工作。另一方面，他的电视根本拒绝播放。这是因为近地轨道输出 59.1 帧/秒，而不是标准的 60 帧/秒。使用 FPGA，[Charlie]将 NeoGeo 超频了大约 1%，并使用 27Mhz 像素时钟将 FPGA 输出更改为 720 x 480p 信号。

对于那些喜欢过去的扫描线的人来说，他们可以通过一个按钮来启用。[Charlie]注意到一些图形的阴影效果有一些细微的差异，但他已经尽了最大努力将其最小化。他还承认，与模拟输出相比，FPGA 代码只贡献了 100 微秒的延迟，这对于即使是最铁杆的游戏玩家来说也足够快了。

休息后，请观看视频，了解 Neo Geo 在 HDMI 中的外观，并与 CRT 电视进行对比。

[https://www.youtube.com/embed/bTamCo2C6kg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/bTamCo2C6kg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)