# 将 CT 和 MRI 转换为可打印对象

> 原文：<https://hackaday.com/2014/06/22/converting-cts-and-mris-into-printable-objects/>

人们每天都要接受 CT 和 MRI 扫描，当[奥利弗]需要做一些医学诊断成像时，他肯定会要求这些文件[，这样他就可以把他的头骨变成一个可打印的 3D 物体](http://www.youtube.com/watch?v=FybESyz5LmQ)。

[Oliver]正在使用三种不同的软件将他从放射科医生那里收到的 DICOM 图像转换成合适的 3D 模型。前两个是由犹他大学综合生物医学计算中心开发的 [Seg3D](http://www.sci.utah.edu/cibc-software/seg3d.html) 和 [ImageVis3D](http://www.sci.utah.edu/cibc-software/imagevis3d.html) 。Seg3D 将来自 MRI 或 CT 扫描的所有 2D 图像缝合成适当的 3D 格式。ImageVis3D 允许[Oliver]剥离他的肉层，允许他只导出他的头骨或整个面部的一部分。第三个软件， [MeshMixer](http://www.meshmixer.com/download.html) ，只是一个网格编辑器，可以很容易地用 MeshLab 或 Blender 替换。

[奥利弗]在他的头骨模型上还有很多工作要做——清理网格，移除下颌骨，如果他想打印一个非常非常棒的杯子，可能还要塞住他的脊柱顶部。不过，所有的数据都在那里，在发送出去打印之前，可以进行数字处理。

[https://www.youtube.com/embed/FybESyz5LmQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/FybESyz5LmQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)