# 用火花核心重新训练 led 字幕

> 原文：<https://hackaday.com/2015/03/20/rebraining-an-led-marquee-with-a-spark-trammell-hudsoncore/>

电线？这个 LED 滚动器要去的地方我们不需要电线。嗯，除了权力，但一切都需要权力。90×7 LED 天棚悬挂在纽约市电阻器激光切割室的入口处。多亏了一个火花核心和来自[Trammell Hudson]的一点工作，[这个标志正在工作并连接到网络上](https://trmm.net/SparkSign)。

原始装置需要 RS485 连接进行输入。除此之外，没有真正的理由它一直在收集灰尘。对内部结构的进一步观察证明，显示器的驱动方式完全符合您的预期:晶体管用于行，移位寄存器用于列。实际上，列被分成单独的偶数和奇数移位寄存器，但这不会使事情变得太复杂。GPIO 占用 7 个行驱动晶体管、2 个移位寄存器时钟、数据、锁存和总共 12 个引脚的使能。

Spark 内核通过每天 ping 网络一次来实现 UTC 时间同步，从而完全取代了 Atmel 80C32X2 及其 RTC。

[通过[纽约电阻器](http://www.nycresistor.com/2015/03/15/sparksign/)