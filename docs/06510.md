# 起重机游戏，Oculus 风格

> 原文：<https://hackaday.com/2014/07/08/the-crane-game-oculus-style/>

我们很确定黑客群体是这样一种人，他们看到一台巨大的塔式起重机在天际线上吊起横梁，然后说，“那会很有趣，至少在我去上厕所之前是这样。”意识到拥有这些起重机的人可能不会让任何普通的乔离开街道进入小屋，[托马斯]和[屏幕名称](看到了吧，这就是为什么我们有支架，孩子们)[用 Oculus Rift](http://hackaday.io/project/1689) 建造了他们自己的微型版本。

这些家伙使用的不是数百英尺高的起重机，而是一个小得多的版本，只有一米多高，通过串行连接由计算机远程控制。在小塑料驾驶室的正下方是一块板，上面有两个广角网络摄像头。来自这些摄像机的视频被发送到 Oculus，这样操作者就可以看到吊杆四处摆动，绞盘展开以拾取小物体。

这些家伙还添加了一点 OpenCV 来添加基于颜色的对象检测。这多少有些用处，但是也有一个到物体的距离的近似值，如果你在地面上没有一个三英寸高的观测者，这将是非常有用的。

下面视频。

[https://www.youtube.com/embed/WTd0HjDdIBI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/WTd0HjDdIBI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)