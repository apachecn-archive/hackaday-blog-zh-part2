# 家酿 ECU 增加马自达变焦

> 原文：<https://hackaday.com/2015/07/09/homebrew-ecu-increases-mazda-zoom/>

大多数现代汽车的一个大问题是用户无法维修的零件和系统数量庞大。这与几十年前的汽车大相径庭，当时的汽车设计是为了让车主能够轻松地对其进行改造。为此，[安东尼]又名[fuzz onkey]解决了现代汽车中通常最难解决的问题:[发动机控制单元](https://www.youtube.com/watch?v=xL8I9Unyhc4)。(关于这个项目的旧帖子可以在【安东尼】的[旧项目日志](http://fuzzymonkey87.blogspot.com.au)中找到。)

任何现代汽车中的每个传感器都由一台名为发动机控制单元(ECU)的计算机监控，计算机负责获取这些数据，并就汽车应该如何运行做出决定。理论上，一个定制的 ECU 能够改变汽车的任何行为，但实际上这是非常困难的，因为计算机需要大量的操作，而且现代发动机的公差非常特殊。

安东尼为他的马自达 MX-5(北美的 Miata)创建的定制 ECU 基于 PIC18F46K80 微控制器，实际上有两个单元。第一个处理时间敏感的操作，如监控发动机凸轮位置和发动机正时，另一个为主单元生成时钟信号，并监控冷却温度和控制怠速。这两个单元通过 SPI 进行通信。

[Anthony]的定制 ECU 很特别，因为他让他的车跑得很好。有一些缺陷，但希望他会有一个比工厂 ECU 更好的产品，允许他改变任何东西，从油门响应和发动机正时到空燃比。过去也有一些驯服 ECU 猛兽的尝试，但目前为止还没有太多。

[https://www.youtube.com/embed/xL8I9Unyhc4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/xL8I9Unyhc4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)