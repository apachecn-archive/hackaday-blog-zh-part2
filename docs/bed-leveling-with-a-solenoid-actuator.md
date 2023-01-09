# 使用螺线管致动器的床调平

> 原文：<https://hackaday.com/2014/10/05/bed-leveling-with-a-solenoid-actuator/>

啊，打印机床调平的悲哀。除非你有一台漂亮的 3D 打印机，否则整平床铺是一件乏味的工作。[Rupin]厌倦了摆弄他的打印机，所以他决定[制作他自己的床水平传感器。](http://www.youtube.com/watch?v=IcpadyjHqhs)

我们的目标是制造一个 Z 轴探头，既能作为自动调平传感器，又能作为终点挡板。他最初试图使用伺服电机探针设计一些东西，但最终放弃了这个想法，因为电机噪音大，校准困难。

此后，他转而使用带有光隔离器的螺线管致动器来确定位置。该致动器延伸一个 M3 螺钉，该螺钉将接触床-随着位置的调整，每次都可以使用软件来调整床，以获得完美的水平床。

相对而言，这方面的硬件很容易做到。[Rupin]现在正在清理代码，当他对它满意时，他将把它作为打印机固件的马林分支的一部分发布。

[https://www.youtube.com/embed/IcpadyjHqhs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/IcpadyjHqhs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

或者，如果你正在寻找更多的挑战，你可以尝试[使用温度力敏感电阻来调平你的床……](http://hackaday.com/2014/03/19/ask-hackaday-auto-bed-leveling-and-high-temperature-force-sensitive-resistors/)