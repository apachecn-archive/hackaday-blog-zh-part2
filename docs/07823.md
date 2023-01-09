# 在乌库勒的带领下踮着脚穿过郁金香

> 原文：<https://hackaday.com/2014/12/17/tiptoe-through-the-tulips-in-no-time-with-ukule-led/>

听一个弹了 20 多年吉他的人说:看乐谱可能是享受音乐的一大绊脚石。靠耳朵演奏有些不可靠，只有在你已经熟悉曲调和速度的情况下，琴谱才能发挥作用，从和弦图上提取旋律就像从字典中编织小说一样。了解基本的和弦构成有很多好处，但让你的手指模仿你在页面、屏幕或其他人的指板上看到的东西可能很困难。进入 [Ukule 主导的](http://people.ece.cornell.edu/land/courses/ece4760/FinalProjects/f2014/ras578_yt336/ras578_yt336/index.html)，这是康奈尔大学【Raghav 和 Jeff】的一个学习工具和全面的酷项目。

Ukule-LED 在指板的前四个位置使用 16 个新像素来教授和弦位置。所有 16 个 NeoPixels 都串联到 ATMega1284P 上的一个引脚，atmega 1284 p 位于一块电路板上，该电路板与电源和串行线一起安装在 uke 的底部。[Raghav 和 Jeff]将新像素设置在表面以下，以便不中断可玩性。uke 可以在“游戏”和“练习”两种模式下运行。在“播放”模式下，用户输入一个代表歌曲和弦、速度和拍号的文本文件。led 实时显示和弦变化，就像手指的卡拉 ok 提词器。在“练习”模式下，用户通过 CLI 输入和弦，灯光保持稳定，直到获得新的分配。知道在哪里使用哪个手指取决于用户。

为了增加另一层学习，大和弦以绿色点亮，小和弦以红色点亮，第七和弦以蓝色点亮。这些是当前支持的 chord 类型，但该项目是用开放的、高度可扩展的 Python 巫术构建的，可以下载并随后进行修补。休息后继续巡演。

[https://www.youtube.com/embed/ZFSE3w9A93U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ZFSE3w9A93U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)