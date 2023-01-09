# 在通过验证的图像中隐藏可执行 Javascript

> 原文：<https://hackaday.com/2014/11/15/hiding-executable-javascript-in-images-that-pass-validation/>

这里有一个有趣的概念验证，根据您遇到的情况，它可能有用，也可能有害。[jklmnn]从[Ange Albertini]的工作中获得了灵感，Ange Albertini 记录了一种在. gif 文件头中隐藏 Javascript 的方法。它不仅包含完整的代码，而且图像和 Javascript 都被视为有效。

只需做一点点工作[jklmnn] [就能把这个概念浓缩到最基本的部分](http://jklmnn.de/imagejs/)以便于理解。接下来，编写了一个快速程序来自动嵌入 Javascript。[如果你想自己试一试，就抓取源代码](https://github.com/jklmnn/imagejs)。

让我们回到为什么这是有用的而不是有害的。如果你在一台不允许浏览器加载 Javascript 的电脑上工作怎么办？你可以嵌入一些有用的东西，就像黑客通过滥用微软 Excel 允许电影播放一样。