# 拳击教练使用 DIY 力传感器

> 原文：<https://hackaday.com/2014/12/21/boxing-trainer-uses-diy-force-sensors/>

康奈尔大学的一组学生设计并建造了他们自己的[电子拳击训练器](http://people.ece.cornell.edu/land/courses/ece4760/FinalProjects/f2014/fx28_tcc54/ece4760_website/index.html "Electronic boxing trainer")系统。他们的工作成果是一个类似打地鼠的游戏。有五个方形垫，大致组织成人体躯干和头部的形状。每个衬垫将根据预编程的模式点亮。pad 亮了，就该玩家出拳了！这个游戏记录了玩家的准确性和反应时间。

该团队试图将预算控制在 100 美元以下，这意味着现成的组件成本太高。为了解决这个问题，他们设计了自己的力传感器。这些传感器基本上是几种不同材料的三明治。中间是一个 10 英寸乘 10 英寸见方的 ESD 泡沫。压在它上面的是 1/2 英寸厚的绝缘泡沫橡胶。这种泡沫橡胶片上有 1/4 英寸的切口，看起来像监狱的栅栏。夹在这两片泡沫之间的是精致的铝纱窗。铜线是用导电胶固定在屏幕上的。最后，整个东西被夹在扁平的瓦楞纸板之间，以保护屏幕。

传感器平放在墙上。当用户击打传感器时，它会压缩。这种压缩导致两片铝屏之间的电阻发生变化。可以测量电阻来检测击中。学生们发现，如果传感器受到更大的冲击，更多的表面区域会被压缩。这导致阻力的更大变化，然后可以被测量为更有力的撞击。不幸的是，它需要根据撞击传感器的物体进行校准，因为撞击物体的大小会影响校准。

每个感应垫都被一条 led 包围着。发光二极管亮起，指示用户应该点击哪个键盘。一切都由 ATMEGA 1284p 微控制器控制。这是来自康乃尔大学的[学生项目](http://www.hackaday.com/2014/12/20/electronic-glove-detects-sign-language "ASL Glove")系列中最新的一个。请务必观看下面的演示视频。

[https://www.youtube.com/embed/642w2c7zcCM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/642w2c7zcCM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[谢谢布鲁斯]