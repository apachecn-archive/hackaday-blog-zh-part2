# 黑进一个便宜的玩具四轴飞行器和 Arduino 一起工作

> 原文：<https://hackaday.com/2013/11/19/hacking-a-cheap-toy-quadcopter-to-work-with-arduino/>

建造自己的四轴飞行器是一项昂贵而微妙的考验。只有在您浏览了一系列不同的项目构建之后，您才会有足够的信心开始购买部件，如果您的目标是直接投入到一些黑客活动中，那么投资可能不值得。幸运的是，[Dzl]为我们提供了一条捷径；他对廉价玩具四轴飞行器的通信协议进行了逆向工程，使其能与 Arduino 一起工作。

问题中的廉价玩具是来自 Hobbyking 的这个，你可以在[他们的产品演示视频](http://www.youtube.com/watch?v=e5NNDgr2pc4)中看到它飞来飞去。[Dzl]打开附带的控制手持器，找出它使用的收发器，然后找到相关的数据手册，并计算出 SPI 通信中涉及的所有引脚配置。飞行数据以每 20 毫秒发送一次的 8 字节数据包的形式传输，控制油门、偏航、俯仰和滚转。

[Dzl]将构建向前推进了一步，[编写了一个 Arduino 库](http://dl.dropboxusercontent.com/u/2248531/blog/HCD/HCD.zip)(直接 Dropbox 下载链接)，它应该能让你跟上进度，让你直接跳到有趣的部分:黑客和实验！休息后看看他的快速视频，然后通过[看这个](http://hackaday.com/2012/12/02/man-tracks-children-using-a-quadcopter/)说服自己需要一个四轴飞行器，省去了它的创造者【保罗】带儿子去公交车站的麻烦。

[https://www.youtube.com/embed/Laibu0cr7Ko?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Laibu0cr7Ko?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)