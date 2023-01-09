# 外星 CAD 软件来自一个平行宇宙

> 原文：<https://hackaday.com/2015/05/29/otherworldy-cad-software-hails-from-a-parallel-universe/>

与昂贵的专业软件包相比，免费 3D 建模软件的世界趋于严峻。此外，当新用户寻求开源或廉价的替代产品时，3D CAD 建模软件的建议似乎会引起轩然大波。与众不同的是，[Matt]开发了自己的开源 CAD 软件包，扭转了我们进行 CAD 的典型方式。

锑是 3D 建模的新视角。与 Blender 的“自由造型”和 Solidworks 的连续挤压和切割相比，锑邀请您将您的模型分解为原始几何图形和与该几何图形交互的操作的网络。

从功能上讲，锑将对象表示为编码原语和操作的节点的图形集合。想要一个圆筒？从一个圆形节点开始，将其管道化为一个挤出节点。需要裁剪一些零件几何图形？尝试用一个或多个原语定义它，然后执行布尔交集操作。用户甚至可以用 Python 编写的自定义脚本编写自己的节点。总的来说，锑拥有类似于 [OpenSCAD](http://www.openscad.org/) 的参数化设计能力，同时它还通过图形而不是基于文本的部件描述来提高可读性。最后，因为零件几何图形本质上是作为一系列指令存储的，所以零件建模过程不会限制输出的分辨率。STL 网格。(想想:基于矢量的图像和基于像素的图像)。

该软件的当前版本可用于 Mac 和 Linux，整个项目是开源的，可在 [Github](https://github.com/mkeeter/antimony/blob/develop/BUILDING.md) s 上获得。(对于精明的软件开发人员来说，项目的大部分是用 Python 编写的，它与用 C++处理的底层例程进行交互，并通过 [Boost 公开。Python](http://www.boost.org/doc/libs/1_58_0/libs/python/doc/) 。)休息之后，与[Matt]一起观看锑工作流程的视频。总而言之，尽管该软件仍处于 alpha 阶段，但它功能强大，而且(对框图迷来说)直观。我们很高兴戴上编程的帽子，尝试来自的 CAD，因为[Matt]创造了“平行宇宙”

[https://player.vimeo.com/video/125111378](https://player.vimeo.com/video/125111378)