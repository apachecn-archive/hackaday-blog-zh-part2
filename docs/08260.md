# 模块化 555 合成器由 MIDI 控制

> 原文：<https://hackaday.com/2015/02/07/modular-555-synth-is-controlled-by-midi/>

[Atdiy and Whisker]又名[The Tymkrs]创造了一个由 MIDI 控制的 8 音符模块合成器。 (YouTube 链接)。该项目旨在突出他们在[Tindie 商店可以买到的一些模块。](https://www.tindie.com/stores/tymkrs/)本质上，合成器是 8 个经典的[雅达利朋克控制台](http://en.wikipedia.org/wiki/Atari_Punk_Console) (APC)音调发生器。每个 APC 由两个 555 芯片组成，而不是原始设计中使用的 556 芯片。APC 被调到[五声音阶，](http://en.wikipedia.org/wiki/Pentatonic_scale)8 个音符覆盖 1.5 个八度音阶。[Whisker]增加了一个电位计，可以同时控制所有 8 个单稳态振荡器。拧动这个旋钮，合成器就会发出我们都熟悉并喜爱的经典雅达利朋克控制台声音。

8 个 APC 输出被路由到与门的 once 侧。与门的另一端连接到 74hc595 移位寄存器。Parallax Propeller 处理器将 MIDI 音符数据转换为串行流，可以通过菊花链连接多个 595 移位寄存器。8 个与门的输出混合成一个组合输出，输出到[tym krs]演播室放大器。

像许多[Tymkrs]视频一样，这个视频以 MIDI 驱动的即兴演奏结束，概述了电路在歌曲中的声音。点击休息时间，查看所有活动！

[https://www.youtube.com/embed/kuG__jFfwHQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/kuG__jFfwHQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)