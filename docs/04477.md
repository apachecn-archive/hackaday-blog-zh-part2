# 黑掉一个翻转点显示器

> 原文：<https://hackaday.com/2013/11/04/hacking-a-flip-dot-display/>

[![](img/61dba27dd487d24dcebbbb8f618e6326.png)](http://hackaday.com/wp-content/uploads/2013/11/687474703a2f2f692e696d6775722e636f6d2f4c786e6b742e6a7067.jpg)

【TeddyDesTodes】在一个著名的拍卖网站上漫不经心地潜伏时，发现了上图所示的宝石，并[对其进行了逆向工程](https://github.com/TeddyDesTodes/Brose-Vollmatrix/wiki/Hacking-the-Brose-Vollmatrix-compact)。这是一个[翻转点显示器](http://en.wikipedia.org/wiki/Flip-disc_display)，准确地说是 Brose Vollmatrix 紧凑型。它由一面是黑色，另一面是黄色的小金属圆盘网格组成，背景为黑色。通电后，光盘翻转显示另一面。圆盘固定在一根轴上，轴上还带有一个小的永久磁铁。靠近磁铁的是一个螺线管。通过给螺线管线圈施加适当的电极性脉冲，磁体将与磁场对齐，同时转动圆盘。

[TeddyDesTodes]将 25 公斤重的显示屏从邮局搬回家后，打开它，发现主控制板正在使用两个 RS422 收发器。因此，他启动了他的总线海盗，开始嗅流量，并注意到几个命令被重复发送。[TeddyDesTodes]停止了传输，发送了这些特定的命令，并惊喜地看到一些点翻转了。从那里，展示东西是小菜一碟。

如果你对此很熟悉，那可能是因为它是在[的一个饰品比赛更新](http://hackaday.com/2013/11/01/trinket-contest-update-5/)中分享的。但是背景细节太有趣了，我们认为它应该有自己的完整特征。你同意吗？