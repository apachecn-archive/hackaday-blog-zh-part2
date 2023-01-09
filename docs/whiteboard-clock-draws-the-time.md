# 白板时钟画时间

> 原文：<https://hackaday.com/2015/02/23/whiteboard-clock-draws-the-time/>

[莫里斯]最近建造了一个时钟，它可以在白板上画出时间。我们过去已经见过很多[时钟黑客](http://hackaday.com/2015/02/14/hat-mounted-clock-requires-mirror-for-wearer-to-tell-time/ "Hat clock")，甚至还有一个[非常相似的](http://hackaday.com/2014/02/13/a-clock-that-plots-time/ "Drawing clock")。看到人们可以想出不同的创造性解决方案来解决同一个问题总是很有趣的。

该器件运行在 PIC16F1454 微控制器上。该项目的代码可在 [GitHub](https://gist.github.com/m-ou-se/7bcdf9b35117730cf043 "GitHub code") 上获得。该微处理器还连接到一个 433 兆赫的接收器。这使得 PC 能够跟踪时间，而不必在电路中包含实时时钟。USB 连接器仅用于供电。所有的安装件都是在 [OpenSCAD](http://hackaday.com/2013/12/11/3d-printering-making-a-thing-with-openscad/ "OpenSCAD") 中设计的，并在 3D 打印机上打印出来。两个伺服系统控制拉拔臂。第三个伺服系统可以升高和降低白板上的标记。这还有一个额外的好处，就是可以将记号笔笔尖放在橡皮头内部。那样的话，同样的两个伺服系统也可以删除书写内容。

这个系统的通信协议很有趣。发射机在[莫里斯的]电脑上显示为调制解调器。他更新时间需要做的就是“echo 12:00 > /dev/whiteboard”。在这种情况下，cron 作业每 5 分钟运行一次该命令。这使得调整白板上的时间更新速度变得很容易。所有的交流都是单向的。绘图电路将在每次收到消息时验证校验和。如果检查失败，电路只是等待另一个消息。计算机将信息多次传输，以防传输过程中出现问题。