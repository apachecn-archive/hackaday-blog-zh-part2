# LED 机箱灯反映 CPU 的使用情况

> 原文：<https://hackaday.com/2012/05/01/led-case-lights-reflect-cpu-usage/>

![](img/21b1a644bb85a7a8aa5989df50c291f2.png "cpu-usage-LED-indicator")

许多 Linux 用户在他们的状态面板中包含了系统监视器信息，这样他们就可以看到 CPU 何时开始工作。[Kevin]通过根据 CPU 的使用情况改变他的机箱灯[将这个概念更进一步。上面你可以看到绿色、橙色和品红色，但是[Kevin 的]实现使用了全光谱的颜色。](http://cuznersoft.com/wordpress/?p=164)

该项目基于 ATmega48。它运行 V-USB 堆栈，并连接到主板的内部 USB 端口之一。这使他可以轻松地将 CPU 使用数据推送到微控制器，并在那里转换成颜色。机箱正面的每个风扇面板后面都安装了一个 RGB LED，上下各有一个白色 LED 作为强调。通过一些金属氧化物半导体场效应晶体管的脉冲宽度调制，他可以混合和匹配正确的颜色。他通过 PSU 轨道而不是 USB 来给插件供电，这样当电脑进入待机状态时它就会关闭。

不要错过[Kevin]对该系统的解释，以及休息后的运行演示。

[https://www.youtube.com/embed/QuB0xMm1aho?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/QuB0xMm1aho?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)