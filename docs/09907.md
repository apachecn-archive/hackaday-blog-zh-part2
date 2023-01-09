# 来自电子废弃物的热线数控泡沫切割机

> 原文：<https://hackaday.com/2015/08/24/hot-wire-cnc-foam-cutter-from-e-waste/>

在旧货店，几个旧的 DVD ROM 驱动器和一个小型照片打印机是相当标准的东西，但是你怎么处理它们呢？当然，把它们劈成一块[数控泡沫切割机！](http://www.instructables.com/id/Mini-CNC-Foam-Cutter/)

[Jonah]从几个 LITE-ON 品牌的 DVD RW 驱动器开始，它使用步进电机，而不是普通的老式 DC 电机。这是一个巨大的分数，因为步进器使精确定位成为可能。随着内部框架的拆除，螺杆和螺母用于保持两个单位相互平行，形成 Z 轴。

佳能紧凑型照片打印机的进给机构用螺栓固定在底部，形成 Y 轴。在 DVD rom 的激光组件曾经存在的地方添加一点镍铬合金线作为切割元件(这可以在旧吹风机中找到),你就完成了机械加工。

控制由 Arduino 和一些简单的驱动模块处理，以便与步进机接口。g 代码由 CamBam 生成，它可以处理各种 cad 文件，或者有自己的几何编辑器。

从几个方面来说，这是一个让你双脚沾水的绝妙方法；打开东西收获零件，用简单的微控制器驱动步进机，建模和生成 g 代码，等等。我们看到的这个构建的一个问题是先有鸡还是先有蛋的问题，因为你需要将一个泡沫立方体切割成稍微严格的尺寸，然后它才能适合这个切割器。但是我们认为这实际上只是一个迭代设计的问题。

[https://www.youtube.com/embed/AJWd1320AyE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/AJWd1320AyE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)