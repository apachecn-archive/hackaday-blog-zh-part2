# 用 OpenCV 和 DLL 注入技术实现超六边形的跳动

> 原文：<https://hackaday.com/2015/02/28/beating-super-hexagon-with-opencv-and-dll-injection/>

每隔几个月就会有一款令人上瘾的游戏出现，玩家似乎爱不释手——不管它有多令人沮丧。去年其中一个游戏是超级六边形。在经历了几个关卡后，[瓦尔]决定[设计一个机器人来打败游戏](http://crackedopenmind.com/portfolio/super-hexagon-bot/)会比自己动手更有效率。我们自己也玩过几轮超级六边形，我们不能在这方面指责他！

就其核心而言，[超级六边形](http://superhexagon.com/)是一个简单的游戏。墙壁从屏幕边缘向位于屏幕中心附近的船移动。玩家使用箭头键来“环绕”一个中心形状的船。避免被墙壁压碎，你就是黄金。然而，整个游戏板在不停地旋转、膨胀、收缩、闪烁，通常会让玩家迷失方向，同时更复杂的墙壁图案会进来杀死你。简而言之，Super Hexagaon 让头后子弹地狱游戏看起来像是小菜一碟。

打败游戏的第一步是抓屏。[瓦尔]尝试了弗拉普斯和 VLC，但滞后 2 秒或更多是行不通的。然后【Val】转向 DLL 注入。超级六边形调用 OpenGL 函数 glutSwapBuffers()实现[双缓冲](http://en.wikipedia.org/wiki/Multiple_buffering)。游戏的每一帧都在后台渲染。渲染完成后，调用 glutSwapBuffers()来交换缓冲区，该过程重新开始。[Val]更改了游戏代码，这样他自己的帧捕获函数将被调用，而不是 glutSwapBuffers()。一旦他捕获完游戏的视频缓冲区，[Val]就调用真正的 glutSwapBuffers()函数。效果非常好。

现在他有了一个图像，[Val]使用 OpenCV 来处理它。虽然游戏在图形上非常嘈杂，但在任何时候都只有几种颜色。想出一种算法来创建墙壁和船本身的二进制图像并不需要太多工作。

从每面墙的中心投射光线穿过屏幕的中心。在穿过另一面墙之前最长的射线将是最佳的逃逸路线。这个简单的解决方案奏效了，但只持续了大约 40 秒。在这一点上，超级六边形将开始抛出更复杂的模式，人工智能将失败。最终的解决方案是创建一个无障碍环境，该环境也考虑了各种接近的墙之间有多少可用空间。这个新版本的人工智能能够打败游戏。

那么这是一种比手工打磨超级六边形更有效的方法吗？既然[Val]现在知道了所有关于 DLL 注入和 OpenCV 的知识，我们当然认为它是！

点击休息时间，查看[瓦尔的]机器人的行动！

[https://www.youtube.com/embed/OyVcokAUj3E?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/OyVcokAUj3E?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)