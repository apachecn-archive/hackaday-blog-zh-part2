# 手语和口语手套

> 原文：<https://hackaday.com/2012/05/04/sign-and-speak-glove/>

这种电线覆盖的手套能够将你的手势转换成语音，并且是无线的。各种传感器包括九个柔性传感器、四个接触式传感器和一个加速度计。柔性传感器完成了大部分工作，监测佩戴者手指关节的对齐情况。接触传感器增加了 flex 传感器数据，有助于区分手指位置相似的字母。加速度计负责解码手位置的运动。他们联合起来检测美国手语字母表中的所有字母。

ATmega644 监控所有传感器，并通过无线发射器将数据发送出去。MATLAB 负责收集通过无线链路传入的数据。它保存它，供以后使用 Java 程序进行分析。一旦这些动作被解码成字母，它们就被组合成句子，并输入到文本到语音的程序中。

你可能已经猜到休息之后会有一个演示视频。

[https://www.youtube.com/embed/Mt8RCyzaQ_4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Mt8RCyzaQ_4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)