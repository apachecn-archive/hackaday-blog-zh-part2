# 比 Siri 语音识别更好的 Arduino

> 原文：<https://hackaday.com/2013/12/31/an-arduino-with-better-speech-recognition-than-siri/>

8 位 AVR 微控制器 Arduino 的 RAM 少得可怜，闪存空间非常小，实际上没有外设可言，它的语音识别能力比你的 Android 或 iDevice 更好。百分之八十的准确率，相比之下 Siri 只有百分之六十。[这里有视频为证](http://www.youtube.com/watch?v=xpJXD2z8eWs)。

这个由[Arjo Chakravarty] ~~创建的 [uSpeech 库](http://arjo129.github.io/uSpeech/)使用 [Goertzel 算法](http://en.wikipedia.org/wiki/Goertzel_algorithm)~~ 将来自连接到 Arduino 模拟引脚之一的麦克风的输入转换成音素。从那里，相对容易地将这些捕获的音素转化为点亮 LED、转动伺服系统的函数调用，甚至复制 Siri，这是现代版的微软曲别针。

对于 uSpeech 库有一个警告:它只会对预定义的短语作出响应，而不会对正常的语音作出响应。尽管如此，对于一个简单的微控制器来说，这仍然是一个非常了不起的成就。

这不是[我们第一次看到【Arjo】的 uSpeech 库，但这是我们第一次看到它的运行。当这篇文章在几个月前发布时，[Arjo]在中国的防火长城之后，不能发布一个合适的演示。由于 uSpeech 库是一个惊人的成就，我们要求展示一些应用程序的一些视频。没有人付出努力，所以[Arjo]决定利用他的新 VPN 向世界展示他的工作。](http://hackaday.com/2012/09/22/speech-recognition-on-an-arduino)

下面视频。

[https://www.youtube.com/embed/xpJXD2z8eWs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/xpJXD2z8eWs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)