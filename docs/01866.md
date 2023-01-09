# Arduino 变声器把你变成[维德]

> 原文：<https://hackaday.com/2012/10/12/arduino-voice-changer-turns-you-into-vader/>

万圣节就要到了，所以我们当然期待 Hackaday 的读者们为我们准备的一系列令人惊叹的服装。为了让他的声音和服装相匹配，Adafruit 的[Phil Burgess](也是前 Hackaday 校友)组装了一个 Arduino 驱动的变声器，让他的声音有[詹姆斯·厄尔·琼斯]的庄严感或棒棒糖公会成员的轻松感。

如果你曾经玩过唱盘，你会知道以 45 或 78 转/分的速度播放 33 转/分的唱片会让你珍藏的*月亮的阴暗面*变成音调过高的轻松听觉体验。同样，以每分钟 33 或 16 转的速度演奏一首单曲意味着那些曾经美妙的音调现在是在声学地狱中被折磨的灵魂的录音。

[Phil]的变声器也是基于同样的原理工作的，它将来自麦克风的声音录制到一个[环形阵列](http://en.wikipedia.org/wiki/Circular_buffer)中，然后以不同的速率播放出来；如果想要的效果是一个芒奇金，那就快一点；如果今年的万圣节服装是一个西斯尊主，那就慢一点。

完整的构建包括一个 10k pot，用于动态改变变声器的音色，以及一个 [Adafruit Wave Shield](http://adafruit.com/products/94) ，用于播放一些预先录制的光剑碰撞的声音。总之，这是一个非常酷的万圣节服装项目，也是 DSP 和微控制器实时音频修改的很好介绍。

[https://www.youtube.com/embed/eRdSi4gJz98?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/eRdSi4gJz98?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)