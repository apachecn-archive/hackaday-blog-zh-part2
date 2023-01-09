# 解构多氯联苯

> 原文：<https://hackaday.com/2015/03/05/deconstructing-pcbs/>

对电路进行逆向工程最可靠的方法是查看所有元件，这些元件之间的所有走线，然后克隆整个电路。看一看 PCB，你会很快发现这个计划的一个问题:阻焊层隐藏了所有的走线，过孔在元件下面，从一个例子复制一个电路板并不容易。没关系，因为[Joe Grand] [在这里告诉你如何一层一层地解构 PCBs】。](http://www.grandideastudio.com/portfolio/pcbdt/)

这项工作[的大部分最初是在去年 8 月的 DEFCON](https://www.youtube.com/watch?v=O8FQZIPkgZM) 上展示的，但昨天[【乔】在 YouTube 上发布了一系列视频](https://www.youtube.com/playlist?list=PLsyTdiI7kVn-3qh8dHlkTvJLEcsh9TsoR)，展示了去除阻焊膜、多层电路板分层以及使用无损成像检查内部层的不同技术。

如果你处理的是两层板，你最需要做的就是去除阻焊层。这可以通过各种技术来完成，从玻璃纤维刮擦刷到激光烧蚀，再到 T4 的德莱梅尔磨轮。到目前为止，最令人印象深刻和最有效的去除 PCB 上阻焊膜的方法是专业人士的方法:化学方法。在 [Magnastrip 500](https://www.youtube.com/watch?v=Jh3Abq4oMq0&index=25&list=PLsyTdiI7kVn-3qh8dHlkTvJLEcsh9TsoR) 或 [Ristoff C-8](https://www.youtube.com/watch?v=C6Yrv-hOucM&index=26&list=PLsyTdiI7kVn-3qh8dHlkTvJLEcsh9TsoR) 中洗澡会产生完全剥离的木板和充满有毒化学物质的房间。有道理；这是 PCB 工厂在制造过程中需要去除阻焊膜时使用的工具。

去除阻焊膜将得到两层电路板的布局，但如果你要解构多层电路板，你必须将整个电路板分层才能看到内部铜层。到目前为止，最令人印象深刻的方法是使用一台只能被描述为温和暴力的机器，但被动成像技术，如 X 射线、CT 扫描仪和其他足够先进的技术也可以达到目的。然而，声学显微镜或声学显微成像并不成功。[看起来确实很酷，不过](https://www.youtube.com/watch?v=Xn-LifM4lIQ)。

谢谢[莫里斯]的提示。

[https://www.youtube.com/embed/O8FQZIPkgZM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/O8FQZIPkgZM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)