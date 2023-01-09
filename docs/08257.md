# 可爱的小机器人有一双被黑的眼睛

> 原文：<https://hackaday.com/2015/02/07/cute-tiny-robot-gets-a-pair-of-hacked-eyes/>

一天，在我们可怜的无线电室里，[大卫·亨德]买了一个 6 条腿的步行机器人。它带有一个红外遥控器，允许用户从远处控制它的运动。让机器人走了几分钟后，[大卫·亨德]觉得很无聊，认为这将是一个很好的黑客玩具。

他的计划是让机器人自主并能够避开障碍物。首先，机器人被拆开，露出电路板。在那里，他找到了由板载微控制器控制的 ST1155A 双向电机驱动器。在查看了 ST1155A 数据表后，[davidhend]认为他可以用 Arduino 驾驶它。于是，烙铁出来了，所有不必要的元件都从原来的电路板上拆下来了。

一个现成的传感器安装在机器人的前面，负责检测障碍物。这些信息然后被发送回 Arduino Nano，Arduino Nano 控制电机驱动器，使机器人后退、转弯，然后再次开始直线行走，直到检测到另一个障碍。[davidhend]制作了[他的 Arduino 代码](http://www.instructables.com/files/orig/FXY/63GQ/H3QFJP0U/FXY63GQH3QFJP0U.zip)(。zip 文件)提供给任何想做类似项目的人。休息之后请看视频！

哦，如果你打算去小屋拿一个你自己的机器人，你最好现在就去拿。

[https://www.youtube.com/embed/-bUdxV6bGy0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/-bUdxV6bGy0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)