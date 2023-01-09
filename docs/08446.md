# 折纸用跳舞的纸打破了一个动作

> 原文：<https://hackaday.com/2015/03/03/origami-busts-a-move-with-dancing-paper/>

折纸鹤很酷，但你知道什么更酷吗？折纸鹤随着节拍起舞。这就是[Basami Sentaku]在创建[舞蹈论文](https://www.youtube.com/watch?v=05gPzM7OJ34) (YouTube 链接)时接受的挑战。你可能会从他的 [8 位口琴](http://hackaday.com/2014/01/28/the-8-bit-harmonica-blows-in-from-japan/)黑客中想起【巴萨米】。在《舞动的纸》中，纸鹤似乎完全靠自己跳舞——甚至表演一些疯狂的旋转动作。当然，这种“神奇”是由于一些精心编写的代码，以及磁铁，大量的磁铁。

使用磁铁从下面移动物体并不是一个新概念。我们很多人都见过“溜冰池”圣诞装饰，它使用了同样的效果。与滑冰池不同，跳舞纸有活动部件(除了起重机本身)。在塑料表面下是一系列独立控制的电磁铁。每个伴舞者都有一排四个磁铁，而中间的特色舞者有一个 5×5 的矩阵。在田宫电机和变速箱的帮助下，41 个电磁铁缠绕在螺栓上。

实际的舞蹈动作是由运行在 Atmel 微控制器上的 C 代码控制的。当然，微控制器无法驱动那些大线圈，所以一些结实的 TO-220 外壳晶体管被用来切换负载。起重机本身也需要一点修改。细金属丝从它们脚上的钕磁铁一直延伸到起重机的机身。金属丝提供了足够的支撑力来防止纸张折叠，同时又有足够的柔韧性来摇摆。

点击过去的休息，看看舞蹈纸在行动！

[https://www.youtube.com/embed/05gPzM7OJ34?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/05gPzM7OJ34?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)