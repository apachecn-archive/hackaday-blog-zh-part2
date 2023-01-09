# 黑掉克雷奥拉数码灯光设计师

> 原文：<https://hackaday.com/2014/11/24/hacking-the-crayola-digital-light-designer/>

[哈利]写了他对克雷奥拉灯光设计师的的[攻击。Light Designer 是一个非常独特的玩具，让孩子们用红外线光笔在锥形 POV 显示器上书写。[Harry]打开其中一个，发现它有一个旋转的组件，其中有一条 32 个 RGB LEDs 用于显示，还有一条光电二极管用于检测笔的位置。黑客入侵的时机已经成熟。](http://sureoakdigital.com/articles/blog/2014/08/hacking-the-crayola-digital-light-designer-pt1/)

旋转组件使用几个滑环连接来向旋转组件发送功率和数据。[Harry]将逻辑分析仪连接到几个连接上，以确定哪些线路是时钟、数据和帧选择(该条被分成 2 个 16 led“帧”)。他继续对串行协议进行逆向工程，这样他就可以自己驱动这些条了。

[Harry]没有对产品 PCB 上的微控制器进行逆向工程，而是决定使用 Leostick (Arduino Leonardo 克隆)来控制 led 和旋转器。他将 Leostick 安装在旋转组件的轴上，并通过滑环连接为其提供动力。在添加了一些电容以弥补滑环的噪声功率后，[Harry]用自己的控制器启动并运行了 POV 显示器。休息后，请观看视频，了解被黑客攻击的 POV 的运行情况。

[https://www.youtube.com/embed/kamAsletvFc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/kamAsletvFc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)