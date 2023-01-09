# 一个 DIY 的 MIDI 风控制器

> 原文：<https://hackaday.com/2014/09/18/a-diy-midi-wind-controller/>

MIDI 不仅仅是键盘和播放样本的按钮矩阵；几乎所有乐器都有 MIDI 控制器，从吉他到竖琴，甚至是木管乐器。[J.M.]不喜欢现有 wind MIDI 控制器中的功能，[所以他正在开发自己的](http://hackaday.io/project/2992-Hopkins-Electronic-Aerophone)，其功能远远超过任何商业产品。

木管乐器 MIDI 控制器相对简单；在吹口中放置一个压力传感器，并将数据转换为音符开和音符关命令。一些按钮，或者在[J.M.]的情况下，电阻式触摸传感器，可以很容易地映射到乐器的不同指法和音符。Arduino Nano 负责所有这些硬件，2.4 GHz 无线电模块与基站进行无线通信。

一旦到达基站，MIDI 数据可以输出到任意数量的合成器和计算机，但[J.M.] [在设备中添加了一个 MIDI 编解码器芯片](http://hackaday.io/project/2992/log/9651-onboard-audio)，只需一副耳机即可播放。它听起来不太好——大约与旧的声霸卡相同——但凭借风控制器提供的调制和表情控制，它比真正的木管乐器还过得去。

下面的视频。

 [https://www.youtube.com/embed/Dm5FUh7Kzqc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Dm5FUh7Kzqc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/ee8yibxfjww?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ee8yibxfjww?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)