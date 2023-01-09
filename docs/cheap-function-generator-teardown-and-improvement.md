# 廉价函数发生器的拆卸和改进

> 原文：<https://hackaday.com/2015/08/28/cheap-function-generator-teardown-and-improvement/>

总的来说，一分钱一分货，当[Craig]在易贝买了一个便宜的函数发生器时，他并没有对它抱太大期望。但是正如他在他的博客帖子和下面的一系列视频中向我们展示的那样，虽然这台仪器没有达到他的预期，但他还是能够对它进行一些修复。

只花了 100 美元买了 MHS-5200A，[Craig]的冒险是彻底拆卸和分析函数发生器。虽然它有点符合其规格，但很明显，一些设计决策导致了次优的性能。在更高的频率和更高的振幅下，正弦波输出呈现出明显的非正弦特征，更接近于三角形波形。频谱分析仪显示了频谱中的多重谐波。手里拿着逆向工程原理图，他追踪信号产生和调理电路，最终锁定了罪魁祸首——用作最终放大器的运算放大器 AD812。第 2 部分将深入讨论压摆率[，第 3 部分将介绍用更好的选择替换不可靠的芯片](http://www.analogzoo.com/2015/08/mhs-5200a-part-two/)的[，以改善输出信号。我们还处理了低通滤波器的改进，修复了该单元方波函数的严重过冲和振铃问题。](http://www.analogzoo.com/2015/08/fixing-the-mhs-5200a/)

如果黑客攻击 MHS-5200A 对你来说似乎有点熟悉，那是因为我们最近报道了它的另一个逆向工程利用。那个[破解仪器串行协议](http://hackaday.com/2015/07/01/hacking-a-100-signal-generator/)的是【WD5GNR】，也就是 Hackaday 自己的【Al Williams】。为[克雷格]和[艾尔]干杯，他们向我们展示了用一百美元和一点小知识你能做什么。

[https://www.youtube.com/embed/WfC0h8XhA4w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/WfC0h8XhA4w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/rwn5XnT7NVA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/rwn5XnT7NVA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/-xOKNi8M3xE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/-xOKNi8M3xE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)