# 问 Hackaday:不是你妈妈的反馈

> 原文：<https://hackaday.com/2014/11/17/ask-hackaday-not-your-mothers-feedback/>

想象一下，你走在沙滩上，发现一些浮木靠在一堆石头上。你在远处看着它，你的大脑可以毫不费力地判断出你在看什么。你会看到浮木和岩石——你可以毫不犹豫地清楚区分这两种物体。

想想进入大脑的原始数据。岩石和浮木的纹理相似。颜色差不多。不规则形状是相似的。因此，进入大脑 V1 区的两个物体的原始数据也一定是相似的。现在想想将浮木碎片与岩石边缘分开的边界。从原始数据的角度来看，没有边界，同样也没有分离，因为这两个对象非常相似。但是你的大脑可以清楚地看到一块石头和一块浮木——两种截然不同的物体。那么大脑是如何做到这一点的呢？这两者是如何如此容易地区分的？如果木材和岩石分界线两边的原始数据是相同的，那么一定有外部因素决定了分界线的位置。杰夫·霍金斯认为这种外部影响是一种非常特殊和最有趣的反馈。请继续阅读，我们会解释并尝试在不变表征的层级结构中实现这种形式的反馈。

![a heirachy of patterns](img/2eb63d274c86429dcd884781997a6618.png)

我们现在讨论的不是你母亲的反馈。我们不是像神经网络那样简单地将部分输出注入输入。因为我们使用的是模式的层次结构，所以反馈必须发生在层次结构之间。基本上，每个级别都是它上面的父级别的子级别。父级别可以“调整”它下面的子级别实际看到的内容，以适应它预测它(父级别)应该看到的内容。

层次结构的每一层都在不断地试图预测下一个模式会是什么。在很低的层面上，这些只是线条和边缘。但在顶部附近，对高水平模式的持续预测可以作为智能的基础。虽然这只是关于大脑如何做到这一点的许多理论之一，但在硅中复制这种类型的分层反馈应该是可能的。但这并不容易。让我们来看一个简化的例子，它延续了我们之前形成基本形状的不变表示的工作。但这一次，我们将应用分层反馈。

## 用预测寻找结构

在我们前面的[例子](http://hackaday.com/2014/10/27/ask-hackaday-sequences-of-sequences/)中，形成正方形的不变表示，原始二进制数据通过第 4 层进入模型。第 4 层的工作是找到重复的二进制序列，给该序列一个名称，并将该名称传递给第 3 层。第 3 层的工作是找到重复的名称模式，给这组重复的模式起另一个名字，然后把这个名字传递给第 2 层。重复这个过程，直到在最顶层形成正方形的不变表示。

这在一个固定的、不变的环境中工作，没有其他形状或线条来混淆我们的模型。但是，如果我们把正方形和许多其他类似的形状放在一起，试图复制岩石/浮木的问题，会发生什么呢？这就是反馈变得必要的地方。如果我们不能区分正方形的一边和相邻三角形的一边，那么我们必须使用层次结构中较高的正方形的存储不变模式来确定我们看到的是什么。那么我们该怎么做呢？

## 可变性的力量

一个层输出的每个名称都需要一个“调整”变量，该变量由它上面的层控制。例如，假设第 2 层看到模式 115 & 125 经常重复，它给它一个名称 240，并将这个名称传递给第 1 层。时间快进，想象“115”的名字再次出现在第 2 层的寄存器中。它可以以一定的百分比预测它应该看到的下一个名称是“125”。但是说进来的名字更接近“123”。第 2 层将通过更改第 4 层输出的“w”变量来调整第 3 层看到的内容，以便它现在将第 2 层满足其预测所需的内容传递给第 3 层。

这种类型的反馈发生在层次结构的所有阶段之间。这就是为什么你可以清楚地看到浮木和岩石躺在一起，就像你可以看到一个橙色的篮球躺在它们中间一样。虽然识别篮球几乎不需要反馈，但你看到的大部分岩石和木头实际上只是基于岩石和树枝各自不变表示的反馈。同样，我们看不到正方形的一条线与三角形的一条线相邻，因为 ADC 输出的这两条线的数据是相同的。这两个形状只能通过层次结构中更高层的反馈来区分。

请记住，这个简单的工作层次结构的例子仅仅是简单的。在现实世界中运作，一个有效的层级将由数百甚至数千层组成——每一层都有数十万个单独的输入。幸运的是，整个概念可以用软件模拟。有了 FPGAs、千兆字节的 RAM 和每秒可运行数十亿次的 CPU，所有这些都唾手可得，你还在等什么？你能不能写一个程序，把 ADC 中的大量数据配置成一个带反馈的层次结构？你会如何开始？给我们看看你的伪代码草稿。