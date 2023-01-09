# 给你的万用表一个无线遥控显示

> 原文：<https://hackaday.com/2015/02/01/give-your-multimeter-a-wireless-remote-display/>

万用表是硬件黑客的主要工具之一。对于 90%的人来说，仪表引线非常适合测量和查看结果。不过，有时你需要更远的距离，为此，[Ken Kaarvik]发明了[万用表远程显示](https://hackaday.io/project/3525)。当你想测量离工作台几英尺远的东西时，远程显示器非常方便。如果你需要在一个封闭的空间里检查一些东西，比如服务器机架或冰箱，它们也很棒。福禄克实际上出售无线显示万用表，如[他们的 233 型。](http://en-us.fluke.com/products/digital-multimeters/fluke-233-digital-multimeter.html)

这个项目的关键是财富半导体的 [FS9721 LP3 芯片。](http://www.ic-fortune.com/upload/Download/FS9721_LP3-DS-21_EN.pdf) (PDF 链接)FS9721 本质上是万用表的片上系统(SOC)。它包含一个数模转换器、一个 LCD 驱动器和一个微控制器。它还可以通过 2400 波特的串行链路发送数据。[肯]的两个万用表，Digitek DT-4000ZC 和 Fluke 17B，都有这种芯片。Digitek 有一个 1/8”插头用于连接外部世界，而 Fluke 需要一些简单的硬件模块来实现数据输出。

由于这是他参加 EDC 饰品大赛的作品，[Ken]将 FS9721 的串行输出连接到一个 Adafruit Pro 饰品上。小饰品将数据格式化并发送给 nRF24L01+ 2.4GHz 无线电模块。接收端有一个相同的无线电和另一个专业饰品。[Ken]实际上建造了两个无线显示器。一个是双启动游戏男孩前进，它有一个真正光滑的彩色显示器背景。另一个接收器使用 128×64 有机发光二极管。小饰品，nRF24L01+和显示器都整齐地放在一个 Altoids 锡。

点击休息时间后，查看两个无线远程显示器的运行情况！

[https://www.youtube.com/embed/aC0lYVEjQ5c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/aC0lYVEjQ5c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/A0gbS-6kKPo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/A0gbS-6kKPo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)