# 无人机同轴直升机采用独特的驱动机构

> 原文：<https://hackaday.com/2014/12/16/uav-coaxial-copter-uses-unique-drive-mechanism/>

如今，个人无人机变得无处不在，但仍有很大的改进空间。[Modlab]的研究人员明白这一点，他们想出了一种非常独特的方法，只使用两个驱动电机来控制同轴直升机的俯仰、偏航和滚动。

为了只用两个电机控制所有这些变量，你通常需要一个调节螺旋桨叶片螺距的机构。通常这是通过在直升机上安装几个微型伺服系统来实现的。伺服系统通过机械连杆连接到螺旋桨上，因此螺旋桨的螺距可以在飞行中调整。这种方法很好，但是成本高、复杂，并且增加了车辆的重量。

[Modlab 的]系统取消了连杆和额外的伺服系统。他们能够只用两个驱动马达来控制螺旋桨的螺距。螺旋桨使用定制的 3D 打印转子轮毂连接到电机。该轮毂专门设计用于将叶片超前和滞后振荡与叶片桨距变化联系起来。[Modlab]增加了一个与电机当前速度同相的正弦分量，而不是用恒定量的扭矩驱动电机。这允许系统在每次旋转中多次调整叶片的螺距，即使在这些高速下。

一定要看下面的演示视频。

[https://www.youtube.com/embed/aEPf0QHVuMM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/aEPf0QHVuMM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)