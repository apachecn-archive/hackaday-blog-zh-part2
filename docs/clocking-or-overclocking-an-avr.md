# 为 AVR 提供时钟(或超频)

> 原文：<https://hackaday.com/2015/08/04/clocking-or-overclocking-an-avr/>

有些人在他们的车库里制造热棒。有些人把他们的电脑超频到可笑的高时钟频率(咳咳…我们可能偶尔会犯这种错误)。[呆子拉尔夫]决定将 ATTiny13a 推至超过其额定频率两倍的[。](http://nerdralph.blogspot.ca/2015/07/externally-clocking-and-overclocking.html)

看起来并不是很难。[Ralph]使用 44.2 MHz 的 can 振荡器，并设置设备使用外部时钟。他用有点损坏的 UART 进行了测试，只要他将电源电压保持在 5V，它就能工作。他还谈到了一些其他方法来破解外部振荡器，以获得高于股票的频率。

我们不建议在重要或商业项目上依赖超频。可能会有长期影响或微妙的问题。当然，你也不能指望每个部件都以未经测试的频率工作。但是我们真的很有兴趣听听你如何测试这个超频芯片的负面影响。

现在，如果你只是为了运动而这样做，一点点液氮就会将你的 Arduino 推到 65 MHz(见休息后的视频)。我们之前已经讨论过将 20MHz AVR 推至 30 MHz T1，但这比 Ralph 实现的比率要小一些。

[https://www.youtube.com/embed/KVRvWmcxnA0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/KVRvWmcxnA0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)