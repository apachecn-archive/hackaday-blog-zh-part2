# 亚马逊的人工智能逃离了它的硬件监狱

> 原文：<https://hackaday.com/2015/08/04/amazons-ai-escapes-its-hardware-prison/>

现在是 21 世纪，我们距离 60 年代、70 年代、80 年代和 90 年代承诺的语音控制计算机还有很长的路要走。不过，语音交互的状态已经有所改善，亚马逊发布的 Alexa 技能工具包(ASK) 是朝着未来计算机会关注你的方向迈出的又一大步。这使得任何硬件都可以成为 Alexa，你的个人语音助手，能够完成你命令的任何事情。

到目前为止，Alexa 被锁在亚马逊 Echo 中，这个“智能”圆柱体位于你的客厅中，并做你告诉它做的大部分事情。自从亚马逊 Echo 发布以来，我们已经看到 Echo 和 Alexa SDK 用于[开灯和关灯](http://hackaday.com/2014/12/24/home-automation-with-the-amazon-echo/)，控制[Nest 恒温器](http://hackaday.com/2015/07/25/control-nest-devices-with-amazon-echo/)，以及[其他家庭自动化任务](http://hackaday.com/2015/07/16/how-to-make-amazon-echo-control-fake-wemo-devices/)。所有这些构建的背后并不是 Google Now、微软的 Cortana 或者苹果的 Siri 正是亚马逊的 Alexa 将我们带入了一个世界，在这个世界里，《星际迷航》中的[Scotty] [对着一台旧 Mac](https://www.youtube.com/watch?v=hShY6xZWVGE) 说话被视为正常。

现在，[Alexa 技能包的入门指南](https://developer.amazon.com/public/solutions/alexa/alexa-skills-kit/getting-started-guide)更关注网络服务，而不是开灯和关空调。ASK 的示例代码是用 JavaScript 和 Java 提供的，尽管我们认为 Python 的第三方库随时都会出现。如果你想在 Raspberry Pi 或其他小型 Linux 计算机上运行 ASK，你需要一种进行语音捕获的方法；[Jasper 项目](https://jasperproject.github.io/)目前是这一领域的领跑者。

我们希望这能以几种不同的方式改变家庭自动化游戏。首先，ASK 在云端处理所有事情，所以现在非常低功耗的设备已经可以进行一些非常酷的语音交互了。其次，亚马逊开放软件后端的举措意味着，为硬件开发的社区最终可能会向亚马逊施加压力，让系统变得更加开放和透明。

已经在研究 Echo 或 ASK 了吗？[给你的文章发个小贴士](http://hackaday.com/submit-a-tip/),并在下面的评论中告诉我们。