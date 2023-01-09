# PIC32 上的立体声音频

> 原文：<https://hackaday.com/2015/01/11/stereo-audio-on-a-pic32/>

PIC 微控制器是功能强大的小型设备，而[Tahmid]无疑正在拓展这些集成电路的功能。他基于 PIC32 和 microSD 卡制作了一个音频播放器(他指出，这是为了教育目的)。哦，这个基于微控制器的音频播放器也可以播放立体声。

该项目的核心是 PIC32MX250F128B 微控制器。16 位 44.1kHz WAV 文件存储在 microSD 卡上，播放的是令人印象深刻的 12 位立体声音频。也可以回放 8 位文件(有一定难度)。[Tahmid]将接口编程为通过串行端口工作，它非常简洁，主要是因为这是他在微控制器上探索音频的项目，而不是构建他将每天使用的实际独立音频播放器。

不过，即使这个项目还没有准备好取代你的 iPod，如果你想在[Tahmid]的大量工作的基础上继续努力，核心音频处理部分已经完成了。你甚至可以[建立一个像这样的独立音频播放器](http://hackaday.com/2011/04/25/single-chip-digital-audio-player/)，但让它播放高质量的 12 位立体声音频！

[https://www.youtube.com/embed/PLoyxrjAPZo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/PLoyxrjAPZo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)