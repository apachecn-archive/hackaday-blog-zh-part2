# DC 到 DC 转换器的微控制器调整

> 原文：<https://hackaday.com/2015/08/19/microcontroller-adjustment-of-a-dc-to-dc-converter/>

[Hugatry]想用微处理器控制的电压替换 LM2596 降压转换器上的调节电位计。调节器 IC 使用分压器从输出产生 1.25V 基准电压。电位计是设置输出电压的分压电路的一部分。例如，如果分压器为 10:1，控制器会将输出保持在 1.25V，因此，输出电压将为 12.5V

[huga try]的策略是使用来自微控制器的经过滤波的 PWM 信号来抵消 1.25V 信号。通过给控制点增加一个小电压，输出电压就不需要像以前一样升高到 1.25V 基准电压。例如，将 0.25V 电压加到基准输入端只需要 1V 电压，相当于 10V 输出。

该视频很好地展示了 PWM 占空比和输出电压之间的关系。虽然他没有提到，但我们突然想到，由于 PWM 与电源电压成比例，微控制器和 PWM 输出级上的电压可能需要固定。这意味着不能使用降压转换器直接为微控制器本身供电。话说回来，什么样的微控制器需要自己调节电源？

如果您需要复习 DC 到 DC 转换器的工作原理，[我们已经为您准备好了](http://hackaday.com/2015/01/24/a-primer-on-buck-and-boost-converters/)。或者，也许你更愿意用你能想到的最奇怪的方式来测量 PWM。

[https://www.youtube.com/embed/hyLYPu-4EN8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/hyLYPu-4EN8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)