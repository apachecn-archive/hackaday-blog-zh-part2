# 双模雪崩和射频随机数发生器

> 原文：<https://hackaday.com/2014/10/31/dual-mode-avalanche-and-rf-random-number-generator/>

[Paul]设计了一个[新的开放硬件 RNG](http://moonbaseotago.com/onerng/) (随机数发生器)，它在一个小封装中包含了两个熵源。熵的第一个来源是一个典型的雪崩二极管电路，它由一对晶体管组成。该电路产生高速随机脉冲，由板载微控制器采样。

这种设计的独特之处在于第二个熵源:CC2531 RF 接收器。射频接收器不断跳过 2.5Ghz 频段的频道，并测量射频信号电平。信号电平的最低有效位被捕获并用作熵的来源。固件可以配置为单独使用任一熵源，或者组合使用两者。固件还支持可选地白化熵字节流，这在不减少熵的情况下使 1 和 0 的数量均匀。

OneRNG 使用 USB-CDC 配置文件，因此它在大多数现代操作系统中显示为虚拟串行端口。有了 *rngd* 守护进程和一些配置，OneRNG 可以在 Linux 中提供系统熵源。[Paul]也有一篇关于熵发生器背后的[理论的很好的文章，其中包括他的示意图的图像。固件、驱动程序和硬件设计文件是开源的，可以从](http://moonbaseotago.com/onerng/theory.html)[下载](http://moonbaseotago.com/onerng/#downloads)。