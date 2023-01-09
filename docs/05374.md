# 聆听智能音阶

> 原文：<https://hackaday.com/2014/02/22/listening-to-a-smart-scale/>

[Saulius]找不到他想要的经济高效的无线秤，所以他逆向设计了一个现成模型的通信协议，以便自己[获得重量数据](http://lukse.lt/uzrasai/2014-02-building-smart-wifi-enabled-bathroom-scale/)。

[Saulius]买了一台便宜的 Maxim 29-66SH 秤，它使用红外线与可拆卸的数字读数器通信。使用 [USB IR 玩具](http://dangerousprototypes.com/docs/USB_Infrared_Toy)，【Saulius】截获了广播的信息。在一些逆向工程和 Python 脚本的帮助下，他很快发现了他的秤用来编码重量信息的协议。

[Saulius]继续使用 JavaScript、SocketIO 和 Tornado(一个轻量级 Python web 服务器)编写了一个小小的 web 应用程序。通过连接到与 Python 脚本接口的微型网络服务器，监听从 USB IR 玩具接收的秤信息，[Saulius]能够通过网络浏览器在他的智能手机上看到他的体重。

由于所有通信都是通过 IR 进行的，因此无需对秤进行任何干预，因为接收器可以放置在秤本身上发射器视线范围内的任何位置。

查看整个过程的演示视频。如果修补规模还不够困难，[你应该从头构建一个](http://hackaday.com/2013/06/12/building-a-digital-scale-from-scratch/)。

[https://www.youtube.com/embed/vdAChaM0KSI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/vdAChaM0KSI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)