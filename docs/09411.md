# 振动距离手电筒照亮黑暗没有光

> 原文：<https://hackaday.com/2015/06/30/vibrating-distance-torch-illuminates-the-dark-without-light/>

如果你以前曾经不得不在黑暗的房间里走来走去，你就会知道这有多令人沮丧。如果你在一个不熟悉的地方，更是如此。[Brian]试图通过构建一个直观易用的[振动距离传感器](http://www.instructables.com/id/Vibrating-Distance-Sensor/?ALLSTEPS)来帮助解决这个问题。

主电路相当简单。一个 Arduino 被连接到一个超声波距离传感器和一个振动马达上。距离传感器通过计算发出的声音返回传感器所需的时间，使用声音来确定物体的距离。该传感器使用的声音高于人类听觉范围，因此附近没有人会听到它。如果物体非常近，Arduino 就会快速振动电机，如果物体很远，就会缓慢振动电机。整个电路由 9V 电池供电。

这个项目的真正诀窍是整个东西都装在一个旧手电筒里。[Brian]使用 [OpenSCAD](http://hackaday.com/2013/12/11/3d-printering-making-a-thing-with-openscad/) 设计了一个定制的塑料底座。这种安装取代了手电筒的镜头，并允许超声波传感器固定在手电筒的前面。手电筒外壳使得该设备使用起来非常直观。你只需把手电筒指向前方，然后按下按钮。手电筒发出的不是强光，而是震动，让你知道前方是否畅通。这样，用户可以更容易地在黑暗中导航，而没有被看到或吵醒该区域中的人的风险。

这让我们想起了[项目默契](http://hackaday.com/2011/08/19/the-hand-mounted-haptic-feedback-sonar-obstacle-avoidance-asstance-device-or-the-tacit/)，它使用了安装在无指手套上的两个超声波传感器。