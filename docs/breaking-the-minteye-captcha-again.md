# 再次破解 Minteye 验证码

> 原文：<https://hackaday.com/2013/01/19/breaking-the-minteye-captcha-again/>

![cap](img/c63ec0972c5e35771ac8af06b1a93903.png)

几天前，我们在斯图加特的 Shackspace hackerspace 上看到了一篇来自[samuirai]的关于破解 [minteye 验证码系统](http://hackaday.com/2013/01/16/script-defeats-minteye-captcha/)的帖子。像大多数其他验证码破解一样，[samuirai]使用了语音辅助选项，为盲人用户提供音频验证码。使用可访问性选项是一件很棒的工作，但是【杰克】想出了[一个更优雅的方法来击败 minteye 验证码](http://www.jwandrews.co.uk/2013/01/breaking-the-minteye-image-captcha-in-23-lines-of-python/)。

对于那些不熟悉的人来说，minteye captcha 提供了一张通过漩涡过滤器的图片，下面有一个滑块。向左或向右移动滑块来消除漩涡，你就通过了“你是人类吗”的测试。[Jack]没有寻找直线，而是想出了一个在 23 行 Python 代码中轻松击败 minteye captcha 的解决方案:只需最小化 pic 中所有边的长度。

裂缝背后的想法是简单的，你旋转图像越多，图像的边缘就变得越长。边缘检测是一个经过充分研究的问题，因此 minteye 破解脚本需要做的唯一事情就是将验证码的滑块从左向右移动，并测量所有边缘的长度。

[Jack]包括了他破解的图像处理部分的代码，幸运的是省略了他返回 minteye 验证码答案的部分。为此，以及破解验证码的一种非常优雅的方式，我们感谢他。