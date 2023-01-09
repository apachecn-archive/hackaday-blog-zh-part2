# 黑客通过焊接电脑电源制造热探头

> 原文：<https://hackaday.com/2015/07/31/hacker-creates-thermal-probes-by-welding-with-a-pc-power-supply/>

伊利亚·采缅科决定[用裸线制作自己的热电偶](http://xdevs.com/article/k-probe/)。[伊利亚]对测量液氮的温度感兴趣，为此他需要 T 型探头。虽然你可以花大约 20 美元买到这些，但他觉得这对本质上是两根电线的东西来说太贵了，于是决定自己做一根。

热电偶使用[塞贝克效应](http://kasap3.usask.ca/samples/Thermoelectric-Seebeck.pdf)，当一块金属的一端是热的，而另一端是冷的，热端的电子将更加活跃，并向冷端迁移，从而产生电压。虽然这种迁移发生在单一金属中，但不容易测量(因为电压将与测量点相同)。因此，热电偶使用两种迁移速率不同的金属。这种差异产生了一个方向上的整体迁移，并且可以测量与金属相遇处的温度相关的电压。热电偶极其常见，有[多](http://hackaday.com/2013/02/08/building-a-tool-to-measure-melting-point/) [应用](http://hackaday.com/2013/07/16/thermocouple-vacuum-gauge-teardown/)。

为了制造热电偶，[伊利亚]需要将两种金属焊接在一起，并使用 PC 电源和电动工具上的石墨电极组装了一个快速焊接设备。石墨电极很重要，因为它可以防止焊接过程中的氧化。

这一过程运行良好，[Illya]能够制造 K 型和 T 型热电偶，并成功测量低至-190 摄氏度的温度。