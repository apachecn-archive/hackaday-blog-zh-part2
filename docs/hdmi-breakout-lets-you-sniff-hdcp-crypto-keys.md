# HDMI 突破让你嗅 HDCP 密钥

> 原文：<https://hackaday.com/2013/02/18/hdmi-breakout-lets-you-sniff-hdcp-crypto-keys/>

这个黑客有两个真正有用的部分，其中包括[嗅探 HDMI 协议的 HDCP 安全密钥](http://adamsblog.aperturelabs.com/2013/02/hdcp-is-dead-long-live-hdcp-peek-into.html)。第一个是在不中断两个具有 HDCP 功能的设备之间的通信的情况下获取信号。为了做到这一点，[Adam Laurie]首先构建了一条 HDMI 分支电缆，它也可以用作直通电缆。上面看到的电路板被称为 HDMI 螺丝端子板。该图显示了一根电缆在制造过程中自我连接的情况。他所做的是切断 HDMI 电缆的一端，然后使用连续性测试仪来找出哪个螺丝端子与哪个裸线相连。在所有的电线都被计算在内后，带插头的一端连接到他的电视机，第二根电缆连接在电路板的插座和他的 DVD 播放器之间。

他文章的其余部分致力于寻找安全密钥。他在这次冒险中选择的武器原来是一辆巴士海盗，但它运行得有点慢，无法捕获所有数据。他切换到自己设计的工具，在 60MHz PIC32 演示板上运行。有了它，他就能得到密钥，使解密受保护的数据成为可能。