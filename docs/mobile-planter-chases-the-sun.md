# 移动播种机追逐太阳

> 原文：<https://hackaday.com/2014/11/09/mobile-planter-chases-the-sun/>

有两种人:一种人有绿色的大拇指，另一种人杀死他们的仙人掌，因为他们一年多都忘了给它们浇水。可悲的是，我们属于后者。我们目前有一种有弹性的蜘蛛植物，看起来它需要更多的阳光。现在有一种方法可以让它在光线照射的任何地方捕捉到这些光线，这要归功于指示物的[点阵]。她制作了一个移动花盆，可以主动寻找阳光。

种植器的底座由胶合板制成，上面覆盖着假草和一个用来盛放植物的喷壶。花盆底座上面的任何东西都可以修改成任何想要的美感。一个 [CRT 花盆](http://hackaday.com/2012/08/18/crt-reborn-as-a-planter/)可能太重了，但是有无数种方法可以让它个性化。[Dot]用一台 [Afinia](http://www.afinia.com/3d-printers) 3D 打印机用 ABS 塑料制作了各种底座和支架。种植器由 Arduino 微处理器控制，并使用一对 0.5W 的太阳能电池板和视差[【PING】)](http://learn.parallax.com/KickStart/28015)传感器来决定它应该如何从当前位置移动。如果播种机摔倒或撞到向前移动的物体，它会倒车并启动由视差[连续旋转伺服系统](http://learn.parallax.com/KickStart/900-00008)驱动的轮子。它会评估自己的新位置，如果有危险，就重复这个过程。一旦种植器安全了，它就使用太阳能电池板来检测最多的阳光:电池板的总和决定了该区域的亮度，而单个电池板的读数被用来将种植器移向更亮的区域。继续寻找太阳，直到找到阳光最充足的地方(在[代码](http://www.instructables.com/files/orig/F5Z/MXPN/I0RYSCUP/F5ZMXPNI0RYSCUP.ino)中定义)。在这里，播种机在重新启动之前闲置了 10 分钟。

我们认为[Dot]的花盆是一种有趣的方式，可以让植物不受我们的影响而保持快乐和健康。休息之后看一段播种机的视频。

[https://www.youtube.com/embed/y62uKfUb6qM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/y62uKfUb6qM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)