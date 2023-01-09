# 教计算机学习

> 原文：<https://hackaday.com/2012/07/11/teaching-a-computer-to-learn/>

![](img/849498720910eb61e84b03d5f748f66c.png "Chess")

[ukasz Kaiser]设计了一台电脑玩井字游戏。这听起来并不特别，直到你意识到他从来没有告诉他的电脑井字游戏的规则。计算机[在观看了两个人玩游戏的视频后](http://www.extremetech.com/extreme/132558-a-computer-that-learns-the-rules-of-a-game-by-watching-you-play)自己学会了规则([链接到实际论文](http://liafa.jussieu.fr/~kaiser/pub/learning_games_descriptive_complexity.pdf)——PDF 警告)。

[ukasz]用 C++写了一个小程序来识别井字游戏、连接 4 和突破板上的对象位置。这个程序筛选输赢游戏以及非法移动，为相关游戏生成一个类似 Lambda 演算的规则集。尽管[ukasz]只编写了一台计算机来学习简单的游戏，如井字游戏、连接 4 和突破，但他计划升级到更复杂的游戏，如国际象棋。

事实上,[ ukasz]给计算机编程来真正学习游戏规则让我们停下来；在 1964 年[理查德·费曼]给大一物理系学生的一次精彩讲座中，国际象棋这个话题被提了出来。[费曼]将学习国际象棋和进行研究相提并论。每一步都是假设检验，当一个非常奇怪的举动发生时——比如阉割、顺带和提升一个棋子——游戏规则的理论就必须被改写。同样，当物理学中发生极其奇怪的事情——粒子/波二象性和黑洞的存在——科学理论就进步了。

是的，教计算机学习井字游戏的规则似乎无关紧要，但鉴于同样的学习过程可以应用于其他领域，如医学、经济学和几乎所有科学，不难看出[ukasz]的工作有多酷。

通过[极限技术](http://www.extremetech.com/extreme/132558-a-computer-that-learns-the-rules-of-a-game-by-watching-you-play)