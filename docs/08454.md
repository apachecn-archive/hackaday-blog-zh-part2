# 下一场骗局的人脸识别

> 原文：<https://hackaday.com/2015/03/04/face-recognition-for-your-next-con/>

[jwcrawley]正忙着为 8 月底在印第安纳州布鲁明顿举行的大会做准备。工作中的一个问题是看门；最好能知道有多少人，不能重复计算人数。以前，志愿者用枯树来估计有多少人出现。今年，他们可能会采用更具科技感的解决方案:[面部识别和跟踪](https://crankylinuxuser.wordpress.com/2015/03/01/uwho-face-recognition-and-tracking-program/)。

[这个项目名为 uWho](https://github.com/jwcrawley/uWho) ，它使用 OpenCV 中的 faceRecognizer 类。整个项目的目的是从先前的帧中识别出某人是谁。如果程序不知道你的脸，你的相似度——确切地说，是几个数据点——会被添加到人脸数据库中。这很简单，而且根据[jwcrawley]的说法，这很有效。

虽然从技术上来说，这是统计有多少独特的人出现在 Makevention 上的最佳方法，但会有一些讨论来看看这种解决方案是否合适。该程序只在本地保存人脸的唯一数据，在网上不做任何事情。这比脸书做的任何事情都要邪恶，但这里有明显的隐私问题。

[链接到 Makevention](http://makevention.org/) 。