# 打造自己的迷你冰箱？

> 原文：<https://hackaday.com/2015/04/03/building-your-own-mini-fridge/>

玩过珀尔帖板吗？它们是非常酷的组件，看起来有点像陶瓷三明治，当你给它们通电时，一边变热，一边变冷！[Joseph Rautenbach]决定尝试用一个制作自己的迷你冰箱——这是当今大多数现代迷你冰箱的典型工作方式。

他使用的帕尔贴板在大约 3.5 安培时产生 12v 的电流，因此大约是 50W，如果你不正确地散热，你可能会在几秒钟内烧坏它。珀尔帖板只关心两侧的温差——如果你不从热侧带走热量，它很快就会过热并自我毁灭。

[乔的]使用一个聚苯乙烯泡沫冷却器作为冰箱，一对计算机散热器和风扇作为珀尔帖板，以及一个他从易贝买的温度 PID 控制器。外部散热器吸收珀耳帖板产生的多余热量，内部散热器帮助将冷却空气分散到聚苯乙烯泡沫冷却器内部。PID 控制器允许他设置一个首选的温度来保持在盒子里，然后控制输出，以保持这种方式。

为了给整个系统供电，他使用了一种经过改造的电脑 ATX 电源——但是如果你在路上，你也可以从你汽车上的 12V 插座供电！

[https://www.youtube.com/embed/ML7tr-2YvR8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ML7tr-2YvR8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

我们之前已经看到过很多珀尔帖板的酷用途，就像这个[吸人能量的 LED 环！](http://hackaday.com/2013/12/02/energy-harvesting-peltier-ring/)甚至比迷你冰箱还要精致——T2——一个真空吸尘器！