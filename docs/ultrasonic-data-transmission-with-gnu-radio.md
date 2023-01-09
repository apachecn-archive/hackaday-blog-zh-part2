# 利用 GNU 无线电进行超声波数据传输

> 原文：<https://hackaday.com/2013/12/10/ultrasonic-data-transmission-with-gnu-radio/>

当我们听到 GNU Radio 在一个版本中使用时，我们首先想到的显然是 Radio。无论是使用极其昂贵的设备还是 USB 电视调谐器加密狗，GNU Radio 都是电磁频谱末端几乎所有东西的完美工具。

然而，GNU Radio 没有理由不能与其他媒体一起使用，正如[Chris]用他在两台笔记本电脑之间的[超声波数据传输向我们展示的。他用一台笔记本电脑的扬声器以 23 kHz 的频率传输音频。它超出了人类的听觉范围，但令人惊讶的是，它能够被连接到另一台笔记本电脑的廉价桌面麦克风接收到。他的 GNU 无线电装置首先将一串文本转换成一个 5 位的数据包，用 FSK 调制，并将信号提升到 23 kHz。在另一端，数据通过反向做同样的事情被解码。](http://www.anfractuosity.com/projects/ultrasound-via-a-laptop/)

该设置能够轻松拒绝所有不在指定频率范围内的音频；在休息后的视频中，[Chris]在讲述他正在做的事情时，成功地传送了“hello world”。

[https://www.youtube.com/embed/H0DKRl8XIcU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/H0DKRl8XIcU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)