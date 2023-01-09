# 在 3D 对象上打印照片级真实感图像

> 原文：<https://hackaday.com/2015/05/13/printing-photorealistic-images-on-3d-objects/>

水纹印刷是一种将胶片上的彩色油墨转移到物体表面的技术。这种薄膜被放在水上，用一种化学物质激活，这种化学物质可以使它附着在被物理推上去的物体上。浙江大学和哥伦比亚大学的研究人员已经将[水文印刷推向了一个新的高度](http://www.cs.columbia.edu/~cxz/publications/hydrographics.pdf) (pdf 链接)。在 8 月份将在 [ACM SIGGRAPH 2015](http://s2015.siggraph.org/) 上发表的一篇技术论文中，他们解释了他们如何开发一种计算方法来创建与物体精确对准的复杂图案。

典型地，使用重复的图案，因为物体拉伸粘合剂膜；在这个主观过程中，任何复杂的东西都会变形。它通常用于装饰汽车零件，尤其是轮辋和格栅。如果你曾经见过没有实际纤维的碳纤维图案，它很可能被应用于水文印刷。

这个黑客的物理设置相当简单:一桶水，一个连接到手爪的线性电机，和一个 Kinect。物体被连接到夹子上。Kinect 会测量其位置和方向。该数据被应用于对象的 3D 扫描，以及要打印到其上的期望纹理图。一个程序创建了印刷过程的虚拟模拟，将特定的图案输出到胶片上，以解决该过程固有的翘曲。然后用普通的喷墨打印机将图案打印到胶片上。

老虎面具是我们个人的最爱，还有豹猫。它们分别说明了使用单次或多次浸入时，表面图案会变得多么复杂。该系统还考虑了各种形状和大小的物体，尽管研究人员承认物体各部分的凹陷程度有物理限制。如果拉得太薄，颜色会褪色或薄膜会裂开。纹理映射现在可以以一种简单而有效的方式在物理上实现，并产生惊人的效果。

[https://www.youtube.com/embed/YlUhPrAqiY0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/YlUhPrAqiY0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

via [ [reddit](http://www.reddit.com/r/EngineeringPorn/comments/35fg8m/computational_hydrographic_printing_siggraph_2015/)