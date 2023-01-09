# 通过 YouTube 传输数据

> 原文：<https://hackaday.com/2015/08/23/transfer-data-via-youtube/>

最初的隐写术可以追溯到公元前 440 年(根据维基百科)，当时一名希腊人在一块木头上写下秘密信息，用蜡覆盖，然后在蜡上写下无辜的文字。一般来说，这个术语意味着在看起来无害的东西中隐藏信息。 [LVDO 项目](https://github.com/m13253/lvdo)(以及最近的 [Windows 分支](https://github.com/Skylion007/LVDOWin))称它是隐写术，但我们不太确定它符合定义。它所做的是将数据转换成视频，你可以像传输其他视频一样传输。知道你用来创建视频的 LVDO 参数的接收器可以提取数据(尽管，很明显，再现并不总是完全无错的)。

我们不确定这是否真的算作隐写术的原因是，从 YouTube 视频示例(未编码)来看，输出视频看起来像雪。它使用离散余弦变换来产生图案。如果你是秘密警察，你可能不知道信息说什么，但你肯定知道它一定是什么。例如，我们会对在有趣的猫视频中编码数据的东西更感兴趣。

这个想法并不是全新的。用录像机磁带备份电脑在俄国非常流行，尽管它从未在美国流行起来(尽管有一些产品做到了这一点，包括为 [Amiga](http://www.hugolyppens.com/VBS.html) 准备的一个)。如果你想知道，是的，[我们以前也讨论过用小猫](http://hackaday.com/2012/02/27/this-image-contains-a-hidden-audio-track/)隐藏数据。

[https://www.youtube.com/embed/b2bLHO5KC34?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/b2bLHO5KC34?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

如果你想看看编码后的视频是什么样子，这里有一个。我们没有破译它(我们没有钥匙)，但是如果你破译了，结果被破解了，不要责怪我们。

[https://www.youtube.com/embed/GbIBPlg7Uo4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/GbIBPlg7Uo4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)