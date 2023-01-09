# 在 8 位微控制器上播放视频

> 原文：<https://hackaday.com/2012/06/25/playing-video-on-an-8-bit-microcontroller/>

![](img/a614d0fe20ab7a86f3b5fd6e107c9f10.png "video")

诺基亚手机的 LCD 显示器已经被大量用作 Arduino 或其他微控制器项目的易于接口的显示器。通常，这些液晶显示器仅用于显示几行文本，或者如果有人觉得很有趣，显示一个小图形。遗憾的是，我们没有经常看到像播放视频这样更复杂、计算难度更大的任务。[Vinod]向我们展示了他在这些小彩色屏幕上播放视频的方式,令人惊讶的是只使用了 ATMega32 微处理器。

构建从使用以前项目的代码将未压缩的图像数据保存在 SD 卡上开始。[Vinod]能够编写一个幻灯片程序，一次一个文件地浏览 SD 卡，并显示每个图像。从那以后，只需使用 Python 脚本来转换。AVI 视频文件转换为未压缩图像，并以 15 帧/秒的速度显示它们。

把这些视频变成有声电影是一个小问题，但在采取了未压缩的。WAV 文件，并将其发送到 ATMega 上的 PWM 引脚上，[Vinod]设法在播放视频的同时播放声音。

结果是能够以每秒 15 帧和 132 x 65 的分辨率播放声音视频。休息之后你可以看看演示视频。

[https://www.youtube.com/embed/rgvySZNpQFI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/rgvySZNpQFI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)