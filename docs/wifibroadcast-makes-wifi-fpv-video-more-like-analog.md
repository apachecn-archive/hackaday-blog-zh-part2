# Wifibroadcast 让 WiFi FPV 视频更像模拟

> 原文：<https://hackaday.com/2015/06/13/wifibroadcast-makes-wifi-fpv-video-more-like-analog/>

普通 WiFi 不是你想从你的四轴飞行器发送视频回你头上绑着的第一人称视角(FPV)护目镜，因为它是为两个无线电之间 100%正确的双向数据传输而设计的。另一方面，模拟视频信号的传输是有损耗的、单向的、一对多的，这就是为什么远程 FPV 航班都倾向于使用老式的模拟视频传输。

当你接近无线电覆盖范围的边缘时，你更关心的是及时获得任何图像，而不是在延迟后正确获得整个视频序列。当 WiFi 正在重新传输数据包，而你的视频正在缓冲时，你的四轴飞行器正在崩溃，你不需要每一帧视频都完美无缺，才能知道如何保存它。最后，优化单向传输系统的两端要比构建必须对称接收和发射的天线容易得多。

这就是为什么[Befinitiv]写了 [wifibroadcast](https://befinitiv.wordpress.com/wifibroadcast-analog-like-transmission-of-live-video-data/) 的原因:让他的 WiFi FPV 视频系统拥有模拟广播的一些优点。

特别是，两个 Raspberry Pis 与可以置于监控模式的 WiFi 无线电相结合，使他能够定制发送的数据包，允许他的设备绕过 WiFi 的确认方案，添加一个[自定义重传例程](https://befinitiv.wordpress.com/2015/02/26/improved-retransmission-scheme-and-multiplexing/)来帮助限制丢失的数据包，甚至允许多个接收器侦听同一信号，以便可以实施[分集接收](https://befinitiv.wordpress.com/2015/05/24/diversity-for-wifibroadcast/)方案。

如果你在飞机或直升机上播放 WiFi 视频，你应该看看 wifibroadcast，看看[Befinitiv]的[3 公里 WiFi 视频试用](https://befinitiv.wordpress.com/2015/05/05/relieable-3km-hd-fpv-solution/)以获取灵感。