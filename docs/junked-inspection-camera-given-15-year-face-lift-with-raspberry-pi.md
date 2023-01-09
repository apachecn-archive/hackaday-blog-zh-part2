# 废弃的检查相机用树莓派进行了 15 年的翻新

> 原文：<https://hackaday.com/2015/08/13/junked-inspection-camera-given-15-year-face-lift-with-raspberry-pi/>

拥有黑客信誉的好处是，家人和朋友总是在寻找他们认为可能对你有用的东西。[Craig Hollabaugh]的女婿发现了一个检查相机，认为这对他的业余爱好工作会很方便。MagniSight Explorer 于 2001 年首次推出。这是很好的表面贴装电路板工作和检查，除了它的模拟 480p 视频是相当过时的今天的标准。所以[克雷格] [使用 35 美元的 Raspberry Pi 2 和 26 美元的 Raspberry Pi 相机模块，将其升级为清晰的 1080P/30 视频和 500 万像素的图像](http://www.spudcentral.com/potd/150807.html)。升级后，该单元现在是 SMT 返工的一个很好的工具。

没有太多的升级，但[克雷格]在 15 分钟的视频中对 MagniSight 的内部结构做了一个很好的概述。他向我们展示了原始的模拟摄像头模块及其视频卡，该模块能够进行一些额外的处理，如黑白输出和反转视频(负片)。正如他提到的，通过树莓 Pi 上的软件，他很容易做到这一点。一个摄像机镜头负责放大和两个轴耦合到它通过平带(橡皮筋？)注意变焦和对焦。镜头前 45 度角的前镀膜反射镜将光路旋转 90 度，以允许镜头/相机“向下看”。在做了一些实验以找到树莓 Pi 相机镜头单元后面的正确焦点后，他用绝缘胶带覆盖相机模块，然后将它粘到旧的相机支架上。在将其连接到 HDMI 显示器上后，结果非常好，他认为他可以轻松地使用尺寸小到 0402 的组件。

他还想再升级几次，让系统变得更好。他计划用一串发光二极管取代现有的紧凑型荧光灯，这将提供更均匀的照明。此外，他可以控制它们的亮度，并有选择地打开或关闭它们，以获得最佳的照明。另一个有趣的升级是将步进电机添加到 X-Y 平移台上，并使它们的移动自动化。在查找电路板文件及其 BoM 后，他甚至可以搜索零件代号，并移动载物台以使零件成为焦点。

[https://www.youtube.com/embed/mWio3V0H_bw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/mWio3V0H_bw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)