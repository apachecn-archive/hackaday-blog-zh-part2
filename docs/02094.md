# 把 Hexbug 蜘蛛变成一个循线机器人

> 原文：<https://hackaday.com/2012/11/12/turning-the-hexbug-spider-into-a-line-following-robot/>

[https://www.youtube.com/embed/quDHhuEsxEg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/quDHhuEsxEg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

你可能对 Hexbug Spider 很熟悉，这是一款在塔吉特百货和沃尔玛售价 20 美元的小型电子机器人玩具。虽然它们可以被命令向前、向后移动，并在一角硬币上旋转，但没有任何外部传感器来使它真正令人兴奋。[Eric]试图补救这一点，并为 Hexbug Spider 设计了一个行跟踪板替代物。

库存蜘蛛有一个小电路板，允许用遥控器控制两个电机。[Eric]取下这块控制板，换上他自己的控制板，由 TI MSP430 微控制器供电。在这块板上，[Eric]包括一对红外发光二极管，能够检测地面上绘制的白线的路径。仅仅用一点点代码，[Eric]就把他价值 20 美元的 Hexbug 蜘蛛变成了一个看起来非常酷的机器人。

[Eric]找到了如何改进他的机器人玩具的方法，但是他使用的 MSP430 微控制器的能力并不局限于他只能跟随线条。通过使用 MSP430 Launchpad，任何人都可以向改进的蜘蛛上传新代码，甚至可以向这个令人毛骨悚然的步行机器人玩具添加新传感器。