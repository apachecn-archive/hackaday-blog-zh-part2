# 准将 1530 数据集得到一个数字计数器

> 原文：<https://hackaday.com/2014/08/09/commodore-1530-datasette-gets-a-digital-counter/>

啊，卑微的准将 1530 数据集驱动。它在美国并不怎么受欢迎，但在相当长的一段时间里，它是欧洲的标准。[DerSchatten13]仍然使用并热爱他的 1530。当一位同事向他展示一些 7 段气泡发光二极管时，他知道自己必须做什么。于是 [1530 数字计数器](http://retrocomputer.umbrellanet.info/index.php?inhalt=moddingDatasette) ( [译](https://translate.google.com/translate?sl=auto&tl=en&js=y&prev=_t&hl=en&ie=UTF-8&u=http%3A%2F%2Fretrocomputer.umbrellanet.info%2Findex.php%3Finhalt%3DmoddingDatasette&edit-text=))诞生了。

[DerSchatten13]从在试验板上构建他的设计开始。他使用 ATtiny2313 上的每一个 I/O 引脚来实现他的电路。磁带运动由一个自制的[旋转编码器](http://en.wikipedia.org/wiki/Rotary_encoder)检测，该编码器连接到原始机械计数器的皮带传动装置上。为了减少引脚数，[德尚 13]在显示器上复用了 led。

现在是最难的部分了，拆下 1530 和机械计数器。[DerSchatten13]粘上一些支架来固定新的 PCB。在一块电路板上重建电路后，他安装了新零件。最终的结果看起来很棒。从外面看，很难看出这个数字计数器不是原装设备。

除了一个例外，数字计数器的操作与模拟装置相同。清除按钮现在有双重功能。按住它保存当前计数。通过打开小数点来指示保存模式。如果用户倒带，当达到保存的计数时，计数器将停止电机。提示保存的程序变得简单多了！

[https://www.youtube.com/embed/qDTp9UVqI10?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/qDTp9UVqI10?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

谢谢[弗兰克]！