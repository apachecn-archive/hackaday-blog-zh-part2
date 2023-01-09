# 检测互联网上的 ASCII 艺术

> 原文：<https://hackaday.com/2012/04/25/detecting-ascii-art-across-the-internet/>

![](img/08e65f22bccaa3563fc6dfa3b6efc0b9.png "ascii")

作为一名网页开发和设计人员，[Victor]有一个习惯，就是在他设计的每一个网页的顶部的 HTML 注释中加入一个非常漂亮的 ASCII 签名。看到别人这样做，他受到了启发，这激起了他的好奇心，想看看还有谁在这样做。他的想法是扫描互联网的一大块区域，看看还有哪些网页在 HTML 评论中有 ASCII 签名。通过大量非常聪明的工作，[Victor]设法抓住了一些有趣的 ASCII 艺术，如果不查看数百万网页的源代码，这些艺术可能会被错过。

从 Alexa 收集了上百万个顶级域名的列表后，[Victor]编写了一个脚本来并行下载所有页面的 HTML。在那之后，只是一个在所有 HTML 文件中检测 ASCII 艺术的问题。有一些早期的 [ASCII 艺术检测算法](http://www.w3.org/WAI/ER/IG/ert/AsciiArt.htm)，但是没有一个适合【Victor】的用例。最好的结果来自于只看至少 3 行长、40 个字符宽的第一条评论(否则签名人不会希望你快速浏览源代码就能找到它)。在丢弃了所有带有 HTML 标签的东西之后，[Victor]有了一个来自互联网上所有网页的 ASCII 艺术的令人敬畏的画廊。

他发现了什么？嗯，有太多的 ASCII 签名需要[Victor]放在他的网页上，但他确实提供了一个他发现的很好的样本。它们大部分是标识，尽管那里有一个 Hypnotoad 和 Aperture Science 岗哨塔。

如果你想试试[Victor]的脚本，他在 GitHub 上提供了[所有可用的东西。](https://github.com/geon/asciiart/blob/master/download.php)