# Arduino Synth 吉他真的很棒

> 原文：<https://hackaday.com/2015/02/25/arduino-synth-guitar-really-rocks/>

[Gr4yhound]一直在用他最近完成的合成吉他摇滚。吉他大部分是使用 Arduino、一些收获鼓垫和一些带状电位计从零开始制作的。下面的视频显示，不仅听起来好听，而且[Gr4yhound]显然也知道怎么玩。

构建的物理部分由两个主要部分组成。吉他的主体是由[gr4y hound]自己自制的 CNC 加工出来的一大块松木制成的。三个圆圈被路由出来，为收获的雅马哈鼓垫，一些布线和操纵杆屏蔽腾出空间。另一个主要部件是吉他琴颈。这实际上是一个乡绅亲和斯特拉特脖子与品删除。

对于电子设备，[Gr4yhound]在 Imgur 上发布了一系列原理图。琴颈上增加了三个软电位计来模拟琴弦。此设置允许[Gr4yhound]在音符开始后调整手指位置。这会产生滑动的声音，您不容易在键盘上模仿。三个鼓垫充当三根琴弦中每一根的触摸传感器。[Gr4yhound]能够同时弹奏每根琴弦，形成和声。

操纵杆保护罩允许[Gr4yhound]为整体声音添加额外的效果。在他的一个[演示视频](https://www.youtube.com/watch?v=YpkzLo6yx_g "demo video")中，你可以看到他使用操纵杆添加效果。Arduino 微处理器充当主控制器，并将音符作为 MIDI 命令传输。[Gr4yhound]正在使用商用 MIDI 转 USB 转换器，以便在电脑上播放音乐。该转换器还允许他通过 USB 为 Arduino 供电，从而无需电池。

[https://www.youtube.com/embed/s3dBox-LB7I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/s3dBox-LB7I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[谢谢怀布伦]