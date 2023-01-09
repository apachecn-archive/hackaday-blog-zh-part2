# 谈论触觉 3D 打印

> 原文：<https://hackaday.com/2014/11/08/talking-tactile-3d-prints/>

细胞生物学教授[Mike]利用 3D 打印和电容感应的魔力，为盲人学生创造了一种解读显微镜载玻片的方法。他的文章集中在一张显示白鱼囊胚有丝分裂后期的幻灯片上，这是一种研究细胞分裂的流行选择。当学生触摸印刷品的某个区域时，电容传感器会触发音频回放，告诉他们自己的感受。

[Mike]从把细胞的 2D 图像变成 3D 打印开始。为了做到这一点，他制作了黑白图像，然后反转颜色，以便 3D 打印的地形能够正确对应。说话部分由 Arduino Duemilanove 和 Spikenzie 语音屏蔽处理。后者的空间有限，但对于[Mike]制作的音频标签来说绰绰有余，这些标签的长度都不到三秒。

2D 文件的硬拷贝可以方便地确保 cap 传感器处于正确的位置。为了做这些，[Mike]切下一些地板保护垫，用铜带覆盖有粘性的一面。这些都是用双面胶带固定在 2D 图像上的。3D 打印位于顶部，由角落的更多家具垫隔开。他给这个科学三明治模型贴上了一个 3D 打印的盲文标签，上面写着“后期”。[Mike]在美国国立卫生研究院的 3D 打印交换网站上制作了参考 STL 文件和其他一些文件。