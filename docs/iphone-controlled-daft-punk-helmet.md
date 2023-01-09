# IPhone 控制的蠢朋克头盔

> 原文：<https://hackaday.com/2014/11/03/iphone-controlled-daft-punk-helmet/>

几年前，[马克]有一台非常大、非常贵的 3D 打印机。蠢朋克头盔过去是——现在仍然是——非常酷的构造，所以通过一点建模,[马克]和他的朋友[亚历克斯]组装了一个模型，并打印出了一个蠢朋克[托马斯]头盔，目的是将其变成一件伟大服装的基石。一些事情阻碍了这个过程，托马斯的头盔被搁置了几年。[快进到几个月前，【Marc】再次接手这个项目](http://uiproductions.blogspot.com/2014/08/daft-punk-thomas-helmet.html)。结果是一个 3D 打印的蠢朋克头盔装载了 320 个 WS2811 发光二极管。

3D 打印头盔建模良好，用聚碳酸酯打印，但用任何基于挤压的打印机，都会有脊和层来打磨，填充，涂底漆和油漆。这项任务交给了另一位朋友[沙吉]，而[马克]则忙于研究电子产品。

护目镜和“耳罩”的 led 是 WS2811 LEDs，但不是我们习惯看到的 SMD 版本。这些是 8 毫米的通孔发光二极管，安装在一片激光切割的丙烯酸树脂上。led 的控制是用 Teensy 3.1 和[【Paul stoff regen】的 OctoWS2811 库](https://www.pjrc.com/teensy/td_libs_OctoWS2811.html)完成的。矩阵连线，安装电池，增加 WiFi 功能，头盔涂漆(非镀铬；不过，这可能会在以后发生)，[马克]有一个可以通过 iPhone 控制的[托马斯]头盔的副本。

如果你想了解更多[马克]的作品，我们几年前在他的 [RGB LED 套装](http://hackaday.com/2010/09/01/led-suit-lights-up-the-night/)和[气动星际旅行门](http://hackaday.com/2010/12/06/star-trek-inspired-pocket-doors/)上贴了些东西。

下面视频。

[https://www.youtube.com/embed/16Zui-_R588?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/16Zui-_R588?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)