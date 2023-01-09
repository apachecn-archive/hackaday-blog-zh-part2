# 用 Python 扩展 EagleCAD

> 原文：<https://hackaday.com/2014/06/30/extending-eaglecad-with-python/>

虽然 EagleCAD 被嘲笑为非开源软件，但它是一款非常受欢迎的原理图和 PCB 布局软件。大部分流行可能是由于令人难以置信的零件库数量——这当然不是 Eagle 必须提供的功能或其可怕的脚本能力。[Rob]受够了 Eagle 中缺乏良好的脚本支持，所以他一直在花时间[让 Eagle 的 ULP 与 Python](http://www.element14.com/community/thread/23445?start=0&tstart=0) 一起工作。他从事这项工作的时间不长，但已经比通常的 Eagle 脚本有用得多了。

下面你可以看看[Rob]的 Python 工具 Eagle 的两个视频。第一个视频通过对齐几个符号和创建一个董事会的轮廓(与适当的曲线！)摘自 DXF 的一份文件。第二个视频展示了这些工具在布置电路板时的价值:想象一下，只需轻点鼠标，数百个 led 和电阻就会自动对齐。太美了。

所有 PyEagle 的东西都可以在[【Rob】的 github](http://github.com/rmawatson/PyEagle) 上获得，包括一个 DXF 进口商、组经理和对齐工具。现在一切都是 Python 了，不用依赖 Eagle 奇怪的 ULP 语言就可以轻松构建自己的工具。

[https://www.youtube.com/embed/_w7CECR7Dv8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/_w7CECR7Dv8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/CFVXop7sGHc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/CFVXop7sGHc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

谢谢[约翰]的提示。