# 宝马远程解锁没有使用安全 HTTP

> 原文：<https://hackaday.com/2015/02/01/bmw-remote-unlock-wasnt-using-secure-http/>

啊，老 HTTP 对 HTTPS。如果你想把人挡在外面，尾随的 S 应该是你做的第一件事，尤其是当你想把人挡在豪华汽车外面的时候。原来[宝马在那个](http://www.heise.de/newsticker/meldung/BMW-ConnectedDrive-gehackt-2533601.html)上搞砸了。

宝马有一个名为 [ConnectedDrive](http://www.bmw.com/com/en/insights/technology/connecteddrive/2013/) 的信息娱乐功能，可以将你最喜欢的应用和服务集成到仪表盘中。您甚至可以使用该系统解锁车辆，该系统是围绕一个包括 GSM 调制解调器和永久 SIM 卡的硬件构建的。一个安全研究小组最近发现，发送给该系统的命令是通过 HTTP(HTTPS 的未加密同类)发送的。这家由德国汽车俱乐部 [ADAC](http://en.wikipedia.org/wiki/ADAC) 雇佣的公司披露了这个漏洞，并且已经推动了一个空中升级来修补这个缺陷。该补丁被描述为“打开”了 HTTPS，这使我们认为它本来就应该被使用，只是在推出时配置不正确。我们会让你在评论中讨论这一点。说真的，这种事是怎么发生的？这无疑给窃贼能够[神奇地解锁高端汽车](http://hackaday.com/2013/06/05/ask-hackaday-how-are-these-thieves-exploiting-automotive-keyless-entry/)提供了更多线索。他们是这样做的吗？

[谢谢法比安]