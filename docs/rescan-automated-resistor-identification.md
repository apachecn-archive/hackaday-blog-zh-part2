# 重新扫描—自动化电阻识别！

> 原文：<https://hackaday.com/2014/02/16/rescan-automated-resistor-identification/>

需要一种快速简单的方法来对数百个随机电阻进行分类？你可以通过自己阅读颜色代码一次做一个…或者你可以让机器帮你做！

当[Robert]面对一堆未分类的电阻器时，他很快决定没有耐心手动分类。因此，他开始使用 OpenCV 编写一个 Android 应用程序来检测和识别电阻颜色代码。问题是，大多数手机在短距离对焦时都有困难——由于电阻非常小，将手机放在更后面会导致色环只有几个像素宽——这对于图像识别来说不是最大的！

因此，他在电脑上重新开始，用一个便宜的 LED 摄像头代替。他用 java 编写了这个应用程序，这样他就可以重用 Android 应用程序的部分代码。它似乎工作得很好——看看下面的视频吧！这将是完美的搭配[你的照明储物箱黑客](http://hackaday.com/2014/02/15/light-your-way-to-the-correct-resistor/)。

[https://www.youtube.com/embed/33-ZbLsykfc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/33-ZbLsykfc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

他计划很快在 GitHub 上发布它，但如果你真的想要，他说你可以在那之前发邮件给他要一份。