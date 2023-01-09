# 婴儿四足机器人，学习走路

> 原文：<https://hackaday.com/2014/10/22/baby-quadruped-robot-learning-to-walk/>

我们都看过那些疯狂的波士顿动力公司运行四足机器人的视频，这些机器人的时速可达 28 英里。这些东西太神奇了，几乎无法想象如何开始建造一个。[Max]热爱他的机器人，想要制造一个四足机器人，但是作为一个机器人爱好者，他没有足够的现金来制造像波士顿动力公司那样的奢侈机器人。相反，他开始通过设计一个稍微慢一点而且便宜很多的四足机器人来弥补这个差距。

所有的机械部件都是他自己设计的。在权衡了不同材料的优缺点后，他决定框架将由 5 毫米的丙烯酸板制成。机器人的主体具有由螺纹杆隔开的丙烯酸树脂肋。12 个 RC 伺服系统组成了所有的关节，每条腿上有 3 个。请注意在这张照片中，有一个伺服立即旋转另一个伺服。为了支撑旋转伺服系统的另一侧，[Max]用环氧树脂固定在一个 T 型螺母上，固定在一个短长度的螺杆上，然后通过滚珠轴承支撑在机架上。简单有效！腿的上部也是由丙烯酸板制成的，而腿的下部是由一个便宜的相机三脚架制成的。橡胶脚确保防滑立场。

所有的伺服系统都由 Arduino Mega 控制。[Max]目前正在写一个草图，它将执行复杂的数学运算，并为我们人类认为理所当然的运动确定协调的伺服运动，如“向前走”。正如你在视频中看到的，[Max 的]机器人不会很快赶上波士顿动力公司的猎豹，但他有一个很好的开始。

这个项目的未来计划包括蓝牙控制和集成预先安装在机器人“头部”的超声波传感器。休息之后看看视频。[Max]正在寻找一些关于他的项目的反馈。我们 HaD 认为这需要一个好名字。来听听评论里的一些建议吧…

[https://www.youtube.com/embed/dK_Mf7zOu04?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=11&wmode=transparent](https://www.youtube.com/embed/dK_Mf7zOu04?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=11&wmode=transparent)

[https://www.youtube.com/embed/FoocUMC23bI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/FoocUMC23bI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)