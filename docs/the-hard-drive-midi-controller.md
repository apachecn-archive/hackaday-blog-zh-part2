# 硬盘 MIDI 控制器

> 原文：<https://hackaday.com/2015/03/02/the-hard-drive-midi-controller/>

[shantea]制造 MIDI 控制器，在成功地尝试了一系列按钮和旋钮后，他决定扩展到更酷的领域。它叫做 Ceylon，实际上是一个从旧硬盘构建的转盘控制器。

与第一个 MIDI 控制器相比，这将是一个精简的版本，只有三个推子，用于吸引眼球的 led，一对用于增益控制的盆，以及六个防破坏按钮环绕的硬盘。硬盘是这场秀的主角，扮演着旋转编码器的角色。

手动旋转时，硬盘会产生几个相位的正弦波。旋转得越快，振幅和频率越高。这些信号太弱，微控制器无法直接采样，对于数字控制——如 MIDI——您不需要读取模拟信号。在 LM339 四通道比较器的帮助下，这些信号被数字化。有了这两个比较器和硬盘输出的 90 度相位差信号，正交编码就相当容易了。

这个 MIDI 控制器的软件基于 [OpenDeck 平台](https://github.com/paradajz/OpenDeck)，一个整洁的系统，允许任何人创建他们自己的 MIDI 控制器和设备。这也是一个伟大的*期待*董事会，似乎表现良好。下面视频。

[https://www.youtube.com/embed/ObLED808kKk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ObLED808kKk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)