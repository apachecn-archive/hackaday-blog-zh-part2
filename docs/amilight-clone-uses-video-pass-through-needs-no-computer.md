# 流光溢彩克隆使用视频直通；不需要电脑

> 原文：<https://hackaday.com/2013/07/10/amilight-clone-uses-video-pass-through-needs-no-computer/>

据我们所知，这些年来我们讨论的所有流光溢彩的克隆产品都有一个共同点。他们需要一台电脑来做图像处理。这个不一样。左边~~右边~~看到的 PCB 就是视频处理所需要的[。这个项目叫做 SCIMO，是一个名叫[Keiang]的黑客的杰作。](http://www.keiang.de/Content-pid-32.html)

内置在 HDMI 标准中的 DRM 很少让我们生气。这是其中之一。因为 [HDCP](http://en.wikipedia.org/wiki/High-bandwidth_Digital_Content_Protection) 和围绕 HDMI 发放的许可【Keiang】没有使用 HDMI 直通。相反，他使用 HDMI 到 S-Video 转换器。该板充当 S-Video 通道，在视频信号继续传输到电视机之前，使用 STM32 ARM 芯片分析信号。它仍然可以产生令人尊敬的画面，但如果他能采用 HDMI 标准，岂不是会更干净？

**更新:**感谢对此的评论。看起来电视正在接收 HDMI 信号。该板由 HDMI 至 S-Video 转换器供电，该转换器本身通过一个分路器将 HDMI 与电视机并行连接。

其他示例在 PC 上使用 Boblight 进行处理，它可以作为一个独立的嵌入式系统来处理。在选择 led 时，它还提供了相当大的灵活性，支持使用 DMX512、WS28xx 或 TM18xx 协议的像素。

[https://www.youtube.com/embed/pd-0qrtwyzk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/pd-0qrtwyzk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)