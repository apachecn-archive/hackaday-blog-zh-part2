# 欺骗口袋妖怪交易

> 原文：<https://hackaday.com/2014/01/02/spoofing-pokemon-trades/>

[Adan]有一个老游戏玩家闲坐着，没有更好的事情可做，他决定用微控制器来研究链接电缆协议。他有一个 Stellaris Launchpad 来完成这项任务，但最初脑子里没有项目。他在串行协议中的这次冒险是[第一代口袋妖怪交易欺骗器](http://www.adanscotney.com/2014/01/spoofing-pokemon-trades-with-stellaris.html)，它允许他在没有两个游戏男孩或奇怪的“朋友”的情况下获得口袋妖怪

Game Boy 链接协议[有非常好的文档记录](http://nocash.emubase.de/pandocs.htm#serialdatatransferlinkcable)(死链接，试试[互联网档案](http://web.archive.org/web/20140410105329/http://nocash.emubase.de/pandocs.htm))，所以从 Game Boy 到 Launchpad 获取数据就像把一个旧的链接电缆连接器焊接到一块 perf 板上一样简单。弄清楚了电子之后，[阿丹]看了看两个口袋妖怪游戏试图交易口袋妖怪时发生了什么。当两个游戏男孩联系在一起时，游戏中有两个选项:交易或战斗。查看“交易”选项后的数据，[Adan]发现了一些可能是被发送的口袋妖怪的数据结构的东西。在发现[之前，他自己对这一切进行了逆向工程，这也是有据可查的](http://bulbapedia.bulbagarden.net/wiki/Pok%C3%A9mon_data_structure_in_Generation_I)。

综上所述，[阿丹]想出了如何用一个小开发板来交易不存在的口袋妖怪。现在他只传输硬编码在 Launchpad 上的口袋妖怪，但很有可能通过 USB 实时传输口袋妖怪的值。

谢谢[丹]发来这个，不，我们不知道上周口袋妖怪帖子的涌入是怎么回事。下面恶搞的视频。

[https://www.youtube.com/embed/KcJ2uRjjCGg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/KcJ2uRjjCGg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)