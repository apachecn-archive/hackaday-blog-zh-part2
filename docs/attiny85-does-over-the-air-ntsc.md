# ATtiny85 在空中传送 NTSC

> 原文：<https://hackaday.com/2015/02/26/attiny85-does-over-the-air-ntsc/>

[CNLohr]已经习惯于使用 ATtiny 微控制器来处理所有事情，他最受欢迎的项目之一就是使用 ATTiny85 来生成 NTSC 视频。凭借一个 2 美元的微控制器和八个引脚，[CNLohr]可以在任何电视上播放文本和简单的图形。他又回来了，[只是这次微控制器没有插在电视上](http://hackaday.io/project/4348-attiny85-does-ntsc-over-vhf)。

本项目中的 ATtiny 使用片内 PLL 超频至 30MHz 左右。再加上几根足够长的电线，这意味着这种芯片可以生成和播放 NTSC 视频。

[CNLohr]提到应该可以使用该板将隐藏式字幕直接传输到电视。如果你正在寻找用 AVR 在显示器上显示文本的最简单的方法，那就是:一个微控制器和两根电线。他无法实际测试这一点，因为他在世纪之交丢失了小电视的遥控器。因为【CNLohr】没有办法在他的电视上启用隐藏式字幕，他无法为这个电路构建明显的应用程序——一个隐藏式字幕 Twitter 机器人。这并不意味着你不能。

下面视频。

[https://www.youtube.com/embed/DJyQi0aUqVQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/DJyQi0aUqVQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)