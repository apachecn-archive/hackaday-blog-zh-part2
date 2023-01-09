# 组合仪表时钟在路上大出风头

> 原文：<https://hackaday.com/2015/07/03/instrument-cluster-clock-gets-the-show-on-the-road/>

有一天在开车的时候，[Esko]注意到速度计上的数字和表盘是制作时钟的绝佳媒介。这是他第一个使用微控制器的项目，他抓紧时间从一辆菲亚特上拿到了仪表组，[用它制作了一个非常独特的计时器](http://www.fiatforum.com/stilo/425751-stilo-b-can-signals-instrument-cluster.html)。

他选择的仪表组来自 diesel Fiat Stilo ,[ Esko]选择它是因为 diesel 版本的转速表几乎完全符合他的计时需求。速度计测量几乎一直到 240 公里/小时，这对于 24 小时时钟来说也很好。有了主要部件的来源，他找到了一个 Arduino 克隆体，然后上路了(打个比方)。这个项目的一个主要重点是将 CAN 总线信号分类。他发现的 Arduino 克隆体内置了这一功能(最终比真正的 Arduino 和 shield 便宜),这很有帮助，但他仍然很难弄清楚所有的信号。

最后，他让一切都工作了，使用集群中的内置伺服电机发出几秒钟的“滴答”声，并使用燃料表记录分钟。[Esko]完成后还将其捐赠给了当地的汽车博物馆，以便其他人也能欣赏这款独特的腕表。一定要看看下面的视频，看看这个时钟的运行情况，如果你正在寻找你可能躺在周围的仪表组的其他用途，一定要看看这个用于视频游戏的仪表组。

仪表盘的机械装置非常棒，而且是大规模生产的。这就是为什么我们自己的[Adam Fabio]能够获得这种类型的硬件，用于他的模拟仪表步进器套件。他只是简单地添加了一个 3D 打印针和一个 PCB 来简化接口。

[https://www.youtube.com/embed/yxl7wD1D-C0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/yxl7wD1D-C0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)