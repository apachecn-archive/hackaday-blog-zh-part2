# 伺服控制的酒杯播放天使的音乐

> 原文：<https://hackaday.com/2012/08/14/servo-controlled-wine-glass-plays-the-music-of-the-angels/>

[https://www.youtube.com/embed/tUNuTgNU-3c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/tUNuTgNU-3c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

Hackaday 论坛上正在酝酿许多很酷的东西。[igor_b]发布了一个他一直在做的项目,该项目使用伺服系统、电机、酒杯和气球来创建一个单杯的 armonica。

玻璃口琴是一系列套在转轴上的碗，通过手指在眼镜边缘滑动来演奏。它们是非常独特的发声乐器，一些[igor]决定只用一个玻璃来模仿的东西。

因为酒杯产生的音符随着液体的体积而变化，[igor]的第一个想法是用泵来改变水位。当他意识到可以通过将气球绑在伺服系统上来取代水时，他放弃了这个想法。

构建的其余部分是一个简单的基于 555 的电机驱动器，一个用 [GoOSC](http://goosc.sourceforge.net/) 编写的手机应用程序，以及一个小型开发板。为了改变他的乐器的音高，[igor]的手机通过 WiFi 向他的电脑发送命令，电脑反过来控制 Teensy，servo，并最终控制玻璃杯中的水位。

这是一个非常酷的造型，但随着水球取代了玻璃杯中更多的液体，音色会有一点点变化。[igor]尝试了一些其他的物体——一个桃子和一个李子——但是使用装满水的气球产生了最清晰的音调。

现在再做几个，把它们连接到 MIDI 键盘上…