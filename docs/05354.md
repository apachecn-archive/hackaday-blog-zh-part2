# 老虎的眼睛——由点阵打印机播放

> 原文：<https://hackaday.com/2014/02/20/eye-of-the-tiger-as-played-by-a-dot-matrix-printer/>

你有一个大的黑客马拉松吗？需要像洛奇一样开始训练蒙太奇？我们不认为你能得到比这个能播放音乐的[点阵打印机更棒的东西了！](http://vimeo.com/58200103)

黑客利用了一个旧的 24 针点阵打印机，它现在是一个 MIDI 兼容的声音发生器。它使用 Atmega8 和 FPGA 连接到原始打印机电路板的不同部分。Atmega8 接收输入的 MIDI 数据，并将其传送到 FPGA，同时驱动进纸和打印头的步进电机。另一方面，FPGA 负责 PWM 来驱动各个打印机引脚。这意味着打印机可以同时播放多达 21 个音符，并且能够接收多达 16 个 MIDI 通道，所有通道都有单独的音量、音高和键速度！

[MIDIDesaster]还有其他几个他们的打印机在运行的音乐示例，包括缪斯(我们最喜欢的一个)的[杜克·核弹主题、](http://vimeo.com/57303383) [歇斯底里](http://vimeo.com/57303777)，甚至还有[超级无敌掌门狗主题](http://vimeo.com/56586038)！

这是一个类似于我们 9 年前共享的这个[打印机合成器](http://hackaday.com/2005/05/31/dot-matrix-synth/)的项目！留下来观看《老虎之眼》吧！但是如果你戴着耳机…把音量关小。

[https://player.vimeo.com/video/58200103](https://player.vimeo.com/video/58200103)[https://player.vimeo.com/video/57960146](https://player.vimeo.com/video/57960146)

[via [Reddit](http://www.reddit.com/r/videos/comments/1ycdng/eye_of_the_tiger_on_a_dot_matrix_printer/)