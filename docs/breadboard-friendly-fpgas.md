# 试验板友好型 FPGAs

> 原文：<https://hackaday.com/2012/12/11/breadboard-friendly-fpgas/>

定期的 Hackaday 读者将会熟悉你可以用 FPGAs 做的所有很酷的事情；即使在您的工作台上有一个普通的 FPGA 开发板，模拟旧的视频游戏控制台、破解加密协议和 DIY 逻辑分析仪也成为相对简单的项目。然而，许多 FPGA 板并不适合原型制作，并且试验板友好型器件很难获得。这是我们在过去几天搜索相关硬件时发现的一对可试验的 FPGAs

首先是[水星 FPGA 模块](http://micro-nova.com/mercury)。Mercury 采用 DIP-64 格式封装，具有相当于 200k 逻辑门的 Spartan-3A FPGA。板上的其他地方是 512kB 的 RAM 和 128kB 的闪存。几乎任何项目都有足够的 GPIO 引脚，但遗憾的是只有 10 位 ADC——与 AVR 或 PIC 'micro 中的分辨率相同。

当然，Mercury 并不是唯一支持试验板的 FPGA 开发板。还有一个稍微更强大的 XuLA2 板，由 Spartan-6 驱动，有 32 MB 内存和 1MB 闪存。与水银不同，XuLA2 还可以安装在那些“半尺寸”的无焊试验板上。

是的，它与普遍推荐的 [Papilio One](http://papilio.cc/index.php?n=Papilio.Hardware) 或 [DE0](http://www.terasic.com.tw/cgi-bin/page/archive.pl?No=593) 有所不同。如果你能推荐任何其他“初学者”(即不花费一只胳膊和一条腿)FPGA 板，请在评论中留下注释，我们将在另一篇文章中总结它们。