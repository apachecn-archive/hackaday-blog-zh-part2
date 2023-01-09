# 语音控制家庭自动化使用 Raspberry Pi 和 LightwaveRF

> 原文：<https://hackaday.com/2013/08/11/voice-controlled-home-automation-uses-raspberry-pi-and-lightwaverf/>

这不完全是人工智能，而是说“Jeeves，lights！”我会打开房间里的灯泡。[Chipos81]围绕着一个 Rapsberry Pi 板建造了声控家庭自动化系统,其中有[lightwaffef](http://www.lightwaverf.com/)装置来开关灯和插座。

LightwaveRF 系统提供 WiFi 链接，为您家中的所有设备提供互联网连接。这使得[Chipos81]从 RPi 控制它们变得轻而易举。为了提供语音识别，他使用了 [CMU 斯芬克斯](http://cmusphinx.sourceforge.net/)。这是一个开源的语音识别库，由卡内基梅隆大学的研究人员开发，在 BSD 许可下发布。在快速解析几组命令的视频中，它似乎做得很好。

“Jeeves”甚至会和你顶嘴确认一个命令。这是由爱丁堡大学开发的包 [Festival](http://www.cstr.ed.ac.uk/projects/festival/) 生成的。这在视频的最后几秒钟提供了一些娱乐，因为我们发现当它说“明天见”时有明显的苏格兰口音。

GPIO 引脚提供一点反馈，使用三种颜色的 led 让您知道系统正在发生什么。甚至还有一个红外 LED 用来给你的电视增加语音控制。

[https://www.youtube.com/embed/gZkwvSX0_Os?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/gZkwvSX0_Os?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)