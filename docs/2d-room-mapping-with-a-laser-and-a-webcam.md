# 使用激光和网络摄像头绘制 2D 房间地图

> 原文：<https://hackaday.com/2014/01/30/2d-room-mapping-with-a-laser-and-a-webcam/>

[Shane Ormonde]最近学会了如何仅使用网络摄像头、激光和每个人都喜欢的数学——三角学——来测量距离。从那以后，他把这个装置放到步进电机上，现在有了一个聪明的 2D 房间测绘机。

他从[Todd Danko]那里学会了如何制作[网络摄像头激光测距仪](http://hackaday.com/2007/04/14/webcam-laser-rangefinder/)，这是我们 7 年前的一个项目！这是一个非常简单的概念。摄像机和激光器以已知的轴间距离相互平行放置。在计算机上，python 脚本(使用 OpenCV 库)搜索图像寻找最亮点(激光)。最亮点离图像中心越近，物体越远。计算从图像中心到激光点的像素可以计算角度，然后可以用来计算到物体的距离——当然，这需要校准才能准确。[谢恩]在他过去的一篇文章中很好地解释了这一切，[建造网络摄像头激光测距仪。](http://shaneormonde.wordpress.com/2014/01/25/webcam-laser-rangefinder/)

从那以后，只需要把测距仪装到步进电机上，用一个小的 PIC 驱动它，然后运行计算程序就可以了！他的成绩相当可观。

[https://www.youtube.com/embed/cejCofAGT7A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/cejCofAGT7A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)