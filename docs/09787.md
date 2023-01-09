# Zynq 和 OPL3 音乐合成器

> 原文：<https://hackaday.com/2015/08/10/zynq-and-the-opl3-music-synthesizer/>

我们是 Zynq 的忠实粉丝，这是一个问题的答案:当你将一个大 ARM 处理器与一个大 FPGA 交叉时，你会得到什么？因此,[ GregTaylor 使用 Zynq 在 FPGA 中模拟 OPL3 FM 合成芯片的项目引起我们的注意也就不足为奇了。

OPL3(也称为雅马哈 YMF262)是老式 PC 声卡上非常常见的 MIDI 芯片。如果你有一个声霸 Pro 或 16 板，你有一个 OPL3 芯片在你的电脑。OPL3 负责了很多你会联想到像《毁灭战士》这样的老式电子游戏的音乐。[格雷格]不仅复制了芯片的功能，还将 imfplay 从 DOS 移植到 Zynq 的 ARM 处理器上运行，这样他就可以重现那些旧的视频游戏声音。

[Greg]使用的 Zybo 板包括 ADI 公司的 SSM2603 音频编解码器，内置两个 24 位 DAC 和 256 倍过采样。然而，与编解码器的接口在代码中是隔离的，因此应该可以很容易地将设计移植到其他硬件上。

为了更好地将原始设备的采样速率与更快的编解码器相匹配，这种设计的运行频率略低于 OPL3，但由于高效的 FPGA 逻辑，新设备可以轻松跟上 49.7 kHz 的采样速率。

使用 FPGA 来模拟 OPL3 可能看起来有些过火，但是[我们见过更糟糕的](http://hackaday.com/2015/03/09/3d-printer-plays-classic-midis/)。如果你更喜欢做你的综合老学校，你可能[得到 555 芯片](http://hackaday.com/2015/02/07/modular-555-synth-is-controlled-by-midi/)的批量价格。

[https://www.youtube.com/embed/KoSF4ZoDuRI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/KoSF4ZoDuRI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/i9vEKyJScYw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/i9vEKyJScYw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)