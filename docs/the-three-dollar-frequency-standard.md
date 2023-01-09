# 三美元频率标准

> 原文：<https://hackaday.com/2015/07/26/the-three-dollar-frequency-standard/>

[Paulie]在 EEVBlog 论坛上，我在易贝买了一个便宜的频率计数器，发现它有点慢。于是，他决定造一个[频标](http://www.eevblog.com/forum/projects/3-dollar-precision-frequency-standard/)。他的建造花费了他大约 3 美元，他分享了设计和软件。

硬件设计非常简单:一个 TCXO(也来自易贝)，一个 ATMega8，一个按钮，和一个带直流到 DC 转换器的 AA 电池来为整个系统供电。该软件完成所有工作，提供从 10MHz 到几百 Hz 的频率(包括一些常见的音频测试频率)。

如果你以前没有使用过 TCXO，它是一个晶体振荡器，包括一个温度补偿电路，可以根据温度升高或降低晶体频率。虽然晶体振荡器已经相当精确，但增加这种温度补偿可以显著提高设计温度范围内的精度(通常比裸晶体振荡器好 10 到 40 倍)。如果你想了解更多关于 TCXOs 的知识，这里有一篇很好的[文章](http://www.radio-electronics.com/info/data/crystals/tcxo.php)。
TCXO 不如 [OCXO](http://hackaday.com/2014/09/15/low-cost-lab-frequency-reference/) (其中第一个 O 代表烤箱)。但是， [OCXOs](http://hackaday.com/2014/07/03/xoxo-for-the-ocxo/) 成本更高，体积更大，消耗电池(毕竟是运行烤箱)。你甚至可以黑掉自己的 OCXO，但它的价格将超过 3 美元。

如果你想见识一下 TCXO 的真面目，可以看看这个视频。

[https://www.youtube.com/embed/kwDsffvTrLk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/kwDsffvTrLk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)