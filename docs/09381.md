# 用 3D 打印机绘制彩色光画

> 原文：<https://hackaday.com/2015/06/26/color-light-painting-with-a-3d-printer/>

光绘，或者拿几个 RGB LEDs，一个长曝光的相机，把世界变成 *Tron* ，已经有一段时间了。我们还没有看到很多人使用他们的家用数控机床达到同样的效果。[ekaggrat]是个例外。他已经用 3D 打印机画了一些浅色的画，[，现在他正在做彩色的](https://hackaday.io/project/6413-sliced-light-in-color)。

这个构建是我们看到的早期项目的扩展，该项目使用白色 LED 在 delta 打印机的构建体积内绘制图片。就像上次一样，[ekaggrat]将 led 连接到一个斜坡板上，并用 M42 命令切换引脚。这种构建只是将布线的复杂性增加了三倍；RGB LED 连接到控制板的引脚 4、5 和 6，他的相机的快门释放按钮通过光隔离器连接到引脚 11。

闪现 Gcode 的能力是一回事，让他两岁的女儿站着不动进行 3D 扫描完全是另一回事。有了这些数据，[ekaggrat]能够通过一个脚本运行这个模型，这个脚本将生成他女儿的一幅浅色画。你可以在 GitHub 上找到脚本，或者看看下面的视频。

[https://player.vimeo.com/video/131520686](https://player.vimeo.com/video/131520686)