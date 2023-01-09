# Arduino 转换方向盘按钮和售后主机之间的信号

> 原文：<https://hackaday.com/2014/09/28/arduino-translates-signals-between-steering-wheel-buttons-and-aftermarket-head-unit/>

毫无疑问，安装在方向盘上的控制装置非常方便。一直走到仪表板上来改变一个广播电台是 20 世纪 90 年代的事情。越来越多的新车配备了立体声方向盘控制，但是，如果你把车头单元换成质量稍高的东西，你就会失去按钮控制。当然，你的汽车/立体声组合可能有现成的适配器，但也可能没有。【Ronnied】走 DIY 之路[自己做适配器](http://hackaday.io/project/3078)。

对[Ronnied]来说，第一个障碍是解决方向盘控制上的布线问题。经过一番摸索，他发现所有的控制按钮只有两根电线，每个按钮只改变两根电线之间的电阻。使用 Arduino 的模拟输入可以轻松读取按钮状态。选择 Pro Mini 型号是因为它的尺寸小，可以放在仪表板的无线电舱中。

下一步是让 Arduino 控制售后市场主机。[Ronnied]对 JVC 的 Stalk 数字控制接口进行了一些研究，但得出的结论是，将 Arduino 输出直接布线到主机电路板上的适当位置会更容易。为了做到这一点，方向盘上的每个功能按钮都被描绘出来，以便在电路板上找到一个共同点。焊接在电路板上的跳线只允许 Arduino 模仿按钮的按动。为了确保主机按钮仍然与方向盘按钮一起工作，Arduino 必须保持 pin 作为输入，直到按下方向盘按钮，pin 变为输出，发送信号，pin 变回输入。这个特性很容易在 Arduino 草图中创建。

下面视频。

[https://www.youtube.com/embed/csXIb0mx8A0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/csXIb0mx8A0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)