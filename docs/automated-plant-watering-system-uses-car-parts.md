# 自动化植物浇水系统使用汽车零件

> 原文：<https://hackaday.com/2015/02/20/automated-plant-watering-system-uses-car-parts/>

[Shane]最近为他的家建造了一个自动植物浇水系统。我们以前见过几个[类似的项目](http://hackaday.com/2014/11/09/solar-powered-circuit-waters-your-plants/ "Plant watering system")，但是没有一个像这个这样运作。谢恩的系统没有连接到房屋管道，也没有使用任何现成的电子阀门。

相反，[谢恩的]建造围绕着一个看起来像是用来喷洒除草剂的装置。该装置的工作方式有点像超级吸水器。用户将水壶装满水，然后多次拉动手柄，以在水壶内建立一些压力。然后可以按下按钮，气压迫使水从喷嘴中流出。[Shane]想出了一种方法来自动化所有这些机械运动。

首先[谢恩]必须找到一种方法来给瓶子打气。他从易贝购买了一个车门电子锁执行器。这是一个非常简单的装置。它只是一台 DC 发动机，带有一个齿轮箱，将发动机的旋转运动转化为直线运动。这是安装在一个木制夹具和连接到泵。一个 dsPIC 微控制器来回旋转电机，依次泵送瓶子。

dsPic 还连接到一个小型伺服系统。伺服机构安装在与车门致动器相同的木制夹具上。一个小臂安装在伺服系统上，当伺服系统旋转时，小臂按下压力释放按钮。这将水从瓶子的喷嘴中送出。[Pat]在喷嘴上接上一小段软管，这样他就可以把水引到他的植物里。下面的视频演示了该装置的工作原理。

[https://www.youtube.com/embed/G9Ij82UbwTI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/G9Ij82UbwTI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)