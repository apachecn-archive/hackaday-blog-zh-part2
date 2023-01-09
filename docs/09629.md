# 3D 鼠标驱动机器人手臂

> 原文：<https://hackaday.com/2015/07/28/3d-mouse-drives-robot-arm/>

你已经造出了完美的机械臂。你如何驾驶它？如果你是[angrymop],你可以通过几个微控制器板从 3DConnexion 连接一个 3D 鼠标。Spacenavigator 鼠标是专业 CAD 人员工作的主要工具，它看起来很适合机器人手臂。

根据[angrymop]的说法，树莓 Pi 可以通过/dev/hidraw(那是原始的人类界面设备)读取鼠标的命令。每个动作产生两行输出。每一行都有一个唯一的识别字节和对应于轴位置的值。

Raspberry Pi 然后使用 SPI 接口与 ARM 微控制器对话，并驱动伺服系统。手臂(机器人手臂，而不是处理器)本身做得很好，由乐高技术部件和常见的钢筋混凝土伺服系统制成。虽然这不是我们见过的用 Technic 建造的最令人惊奇的东西，但它仍然令人印象深刻。

你必须想知道其他的 [3D 控制器](http://hackaday.com/2008/05/30/alternative-3d-controllers/)是否对控制机器人手臂有用，或者太空导航员将如何控制一个[更大、更有能力的手臂](http://hackaday.com/2015/03/14/open-source-robotic-arm-now-within-reach/)。话又说回来，也许这只手臂的大小正适合建造受埃舍尔启发的[。](https://en.wikipedia.org/wiki/Drawing_Hands#/media/File:DrawingHands.jpg)

[https://www.youtube.com/embed/hwWURvjENgM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/hwWURvjENgM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)