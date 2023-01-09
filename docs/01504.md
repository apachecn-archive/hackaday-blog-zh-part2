# 在搅拌机中模拟 LED 立方体

> 原文：<https://hackaday.com/2012/09/03/simulating-led-cubes-in-blender/>

[https://www.youtube.com/embed/bl-kvfJxYwM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/bl-kvfJxYwM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

芬兰的 jyvskyl hacker space hack lab-jlk 有幸为他们的家乡参与了一个公共艺术项目。他们有机会在 jyvskyl 的中央教堂公园设计、建造并安装了三个 LED 立方体。作为这样一个备受瞩目的项目，hacklab-jlk 团队决定慢慢来，最终为他们的 LED 立方体实现了许多非常酷的功能，包括[在 Blender](http://elovalo.org/) 中模拟灯光秀。

LED 立方体与我们之前见过的所有其他 LED 立方体相似；这是一个由 ATMega328 控制的 8x8x8 的立方体。这个名为 Elovalo 的项目由三个 led 立方体组成，一个使用红色 LED，一个使用绿色 LED，一个使用蓝色 LED，每个立方体都安装在 jyvskyl 公园的基座上。

由于 Elovalo 是永久性安装，该团队需要一种方法来验证 LED 立方体的新固件。他们为 Blender 开发了一个 [LED 立方体模拟器](https://github.com/hacklab-jkl/elovalo/tree/master/simulator),允许他们用 C 编写一个新的显示函数，并呈现单帧或完整的照明模式动画。

一个非常酷的建筑，对于一个公共艺术项目来说简直太棒了。我们期待着完整安装的视频，但在此之前，我们将在休息后提供简短的预览视频。

[https://www.youtube.com/embed/bl-kvfJxYwM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/bl-kvfJxYwM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)