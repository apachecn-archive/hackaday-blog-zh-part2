# 遇见 Registroid 突变收银机音乐音序器

> 原文：<https://hackaday.com/2014/12/15/meet-registroid-mutant-cash-register-music-sequencer/>

73 年前，二战正如火如荼地进行着，世界上第一台计算机还没有处理原子弹物理学，百货商店的收银机不得不机械地将你的购买相加。那时候，每次拉动都会使设备像老虎机一样旋转和转动。[大卫]&[斯科特]绑架了其中一辆旧车，[强迫它唱一首新歌](http://monkeycinteractive.com/registroid/)。就这样，Registroid 诞生了，它自称是“变异老式收银机，是一种可播放的交互式电子室内循环机。”为什么还没有其他人想到这一点？

在内部，[增加齿轮和翻滚计数器](http://monkeycinteractive.com/national-cash-register-modification/)被掏空，为电子设备、放大器和扬声器腾出空间。按键被转换成 Arduino 输入，然后馈入 MAX/MSP，作为基本的 midi 控制器。在顶部，五个带 led 的“天线”灯作为一个颜色器官，它们随着由 MSGEQ7 均衡器芯片分割的音频脉冲。每行锁定键对应一种不同的乐器:鼓点、基线、合成器和单拍。

我们以前见过类似的事情发生在游戏机和打字机上，但是提款机对我们来说是新的。也许有一天，有人会扭转潮流，用古董大键琴输入他们的推特信息。

Registroid 在当地活动中展出时似乎很受欢迎，包括一些人想知道密码何时会打开现金抽屉。

[https://www.youtube.com/embed/NTHPurxVJ0U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/NTHPurxVJ0U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)