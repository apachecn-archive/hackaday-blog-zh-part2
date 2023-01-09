# 一个无线网络连接的莫尔斯电码键盘

> 原文：<https://hackaday.com/2015/01/20/a-wireless-web-connected-morse-code-keyer/>

[Kevin]最近在易贝得到了一个 20 世纪 20 年代的莫尔斯电码键盘/发声器。虽然许多火腿喜欢使用 CW 的旧键盘，但[Kevin]采取了不同的路线，将其改造成一个无线网络连接的莫尔斯电码键盘。

[Kevin]在键盘下安装了一个 Arduino Yun，它可以监听用户输入并提供网络连接。云连接到[Kevin]的开源 web API，他称之为“morsel”，这允许它与其他 morsel 用户发送和接收消息[。当一个消息被键入时，Yun 将它发布到 API。当另一个键控器向 API 查询输入信息时，云下载莫尔斯序列并在发声器上重放。](http://morsel.develpr.com/)

[Kevin]还在他的外壳顶部添加了一些铜电极，作为电容按钮，同时保持键控器的老派外观。左按钮播放最近收到的消息，右按钮设置播放速度。休息之后，请观看视频，了解键控器的工作情况。

谢谢你的提示，[Jarrod]。

[https://www.youtube.com/embed/XAbIfIo7n2A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/XAbIfIo7n2A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)