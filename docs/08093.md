# 用 HP 绘图仪绘制电路图

> 原文：<https://hackaday.com/2015/01/18/circuit-plotting-with-an-hp-plotter/>

在过去的几年里，我们已经看到了一些旨在将整条 PCB 生产线放在桌面上的商业产品。这听起来很大胆，上周在 CES 上有几个展位展示了这一点，其中一个从某个博客获得了 5 万美元的支票。[【康纳】和【菲然】决定做黑客版的 PCB 打印机](http://people.ece.cornell.edu/land/courses/ece4760/FinalProjects/f2014/fc254_cwa37/index.html):一台旧的惠普绘图仪改装成现代硬件，配有带导电墨水笔的网络界面。

问题中的绘图仪是一台 1983 年的惠普 HIPLOT DMP-29，像所有旧的惠普设备一样，是科学和工程的杰作。这些电子设备被丢弃(保存下来可能是一个更好的词)并被现代硬件所取代。旧的伺服电机每台大约运行 1.5A，标准的 H 桥芯片和结实的实验室电源这些电机是原始绘图仪中唯一重复使用的部分。为了精确定位，几个 10 转的盆被用胶带绑在电机轴上，并馈入用于控制整个事情的 ATMega1284p。

该版本更有趣的一个方面是 web 界面。这是一个小的 JavaScript 应用程序，能够在 X 和 Y 轴上画线，并将结果坐标从服务器发送到打印机。这很酷，但没有[Connor]和[Feiran]的最终目标酷:使用现有的 Gerber 文件来绘制一些痕迹。他们成功地解析了 Gerber 文件，扔掉了所有多余的命令(训练等)，并用导电墨水绘制出来。

硬件的最终迭代并不完全符合[Connor]和[Feiran]的想法，但这主要是导电墨水糟糕的导电性造成的问题。他们试图通过在每一行上运行笔五次来解决这个问题，但这引入了一些反弹。这是一门*电气*工程课的最后一个项目，所以我们要说没问题。

下面视频。

[https://www.youtube.com/embed/HWdeMJdfJQ0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/HWdeMJdfJQ0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)