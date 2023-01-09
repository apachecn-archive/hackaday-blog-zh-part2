# 模拟屏蔽和 PCB 四轴飞行器

> 原文：<https://hackaday.com/2014/05/30/analog-shield-and-pcb-quadcopter/>

[https://www.youtube.com/embed/gXW76ESIv6k?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/gXW76ESIv6k?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

我们花了一点时间在 Maker Faire 的 TI 展台拍摄了一对采访。第一个是(比尔·埃斯波西托)，他正在攻读博士学位。在斯坦福。他在展示 Arduino 的模拟盾牌。他将其描述为“将模拟工作台引入 Arduino 保护罩的尝试”。我们认为这是一个奇妙的想法，因为大多数通过 Arduino 学习数字电子的人很少或没有模拟电路的经验。这是一个很好的概念入门药物。

[模拟屏蔽](http://analogshield.com)为+/- 7.5 伏、4 通道 ADC、4 通道 DAC 提供良好的电源，并获得 100k 个 16 位样本。他向我们展示了一种频谱分析仪，它对麦克风传入的信号进行快速傅立叶变换。他还在护盾周围建造了一个函数发生器。最后是播放 MIDI 文件的合成器。

在视频的后半部分，我们来看看[Trey German]在基于 PCB 的四轴飞行器上的工作。他的目标是降低功耗，这相当于更长的飞行时间。为此，他选择了 DRV8312 和 Piccolo 来控制每个无传感器无刷 DC 电机。结果应该是比他以前的版本低 10%的功耗。