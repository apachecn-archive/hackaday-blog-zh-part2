# 用发光的雪展示你的城市的情绪状态

> 原文：<https://hackaday.com/2015/02/05/display-your-citys-emotional-state-with-illuminated-snow/>

[Hunter]想为他去年的节日彩灯展示做些更有趣的东西。他想要的不仅仅是动画灯光，而是由数据驱动的东西。在这种情况下，[他的展示](http://www.hscott.net/the-emotional-city/ "Sentiment display")是基于他所在城市的人们的心情。我们在过去见过[非常相似的项目](http://hackaday.com/2013/12/25/christmas-tree-analyzes-your-tweets/ "Sentiment Christmas tree")，但是这次有一些显著的不同。

显示器由 Arduino 驱动。[Hunter]正在使用以太网屏蔽将 Arduino 连接到互联网。然后，它会监控他所在区域 15 英里范围内用户的所有最新推文。这些推文然后被转发到[炼金术情绪 API](http://www.alchemyapi.com/api/sentiment-analysis/ "Alchemy Sentiment API") 进行分析。API 使用各种算法和检测方法来识别文本主体中的总体情感。[亨特]正在用它来确定一条给定推文的文本所表明的总体情绪。

接下来[亨特]需要一种方法来显示这些信息。他选择使用 LED 灯条。由于情绪的范围相当小，[Hunter]不想显示总体平均情绪。这个值在短时间内变化不大，所以看起来没什么意思。相反，他绘制了自上一个样本以来的变化。这导致 LED 显示屏发生更明显的变化。

这个项目另一个有趣的地方是[Hunter]正在用他院子里的雪来散射 led 发出的光。他实际上把长条埋在了一层雪下。这样做的结果是隐藏了电子设备，但模糊了光线，所以你看不到单个的发光二极管。这种效果相当不错，可以为你的节日灯饰增色不少。请务必观看下面的视频进行演示。

[https://www.youtube.com/embed/FGcaexhsqOE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/FGcaexhsqOE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)