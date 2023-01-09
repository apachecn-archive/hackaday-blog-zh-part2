# 逐项列出家庭用水量

> 原文：<https://hackaday.com/2015/05/29/itemizing-water-consumption-at-home/>

有一段时间[Florian]想要详细记录他在家里的用水情况，以便更好地跟踪他的水费账单来自哪里——并帮助他养成节约用水的习惯。他还没有完成，但是已经有了一个很好的开始。

[![Faucet Sensor](img/d28145fb98de75956d88c3e76dd94b1e.png)](http://www.cuddleburrito.com/blog/2015/5/24/itemizing-water-consumption-with-raspberry-pi)

测量你房子里所有东西的用水量的问题是，安装传感器所涉及的管道是一项相当大的工作——所以相反，他假设一些地方的流量恒定，只使用阀门上的传感器来确定阀门打开的时间，这给他提供了一个相当准确的用水量数字。

右边是他的厨房水龙头，它有一个超级快速的街机按钮来跟踪它的开关。

厕所有点棘手。他最终设计了一个 3D 打印的支架，安装在坦克内部的杠杆上——这是非常通用的，所以他包括了。STL 文件，如果有人想尝试实现这个系统。

所有这些交换机都返回到 Raspberry Pi 来跟踪云中的数据，这就是乐趣所在。他对自己得出的一些数字感到惊讶——了解洗生菜沙拉需要多少水，甚至快速洗手需要多少水(大约 250 毫升！)到更不寻常的习惯:

> 此外，这个系统是一个优秀的计时器，记录我便便的时间……也记录其他来参观的人。这会很有趣的。

[![water usage](img/c809b72f6fc1af4303b58669dce66b4c.png)](https://hackaday.com/wp-content/uploads/2015/05/static1-squarespace1.png)

所有这些数据收集也为我们的前进方向提供了一个很好的观点:

> 我最近看了《Ex 玛奇纳》,有一个场景让我印象深刻，它总结了我们正在进入的时代。这个场景是人工智能的创造者描述他在创建第一个原型时的顿悟时刻。他解释说，从人们的互联网搜索中收集的数据不是人们在看什么的地图，而是人们如何看待事物的地图。我们收集的所有数据中有趣的是隐藏在其表面之下的东西。
> 
> 我们越是开始关注眼前的事情，我们就越有可能积极地改变世界。