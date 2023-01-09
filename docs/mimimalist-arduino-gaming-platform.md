# 极简的 arduino 游戏平台

> 原文：<https://hackaday.com/2015/05/27/mimimalist-arduino-gaming-platform/>

一个漂亮的彩色液晶显示屏，一个 Arduino，一个蜂鸣器和一个操纵杆就是你所需要的一个不到 20 美元的极简游戏控制台。至少，这就是[joo vila ca]让这个甜蜜版的俄罗斯方块运行起来所需要的。~~他现在正在努力突破。~~他的突破看起来更好。详见下文附言。

这证明了硬件黑客领域的现状，[joo]可以在一个下午以如此低廉的价格组装这款设备，想必是在等待来自中国的发货一段时间之后。320×240 SPI 彩色 TFT 液晶显示屏的成本是整个项目的两倍。布线很简单，只需将这个引脚连接到那个引脚。几乎是儿戏。

同样令人印象深刻的是开源软件的现状。Seeed Studios 的一个 [TFT 库](https://github.com/Seeed-Studio/TFT_Touch_Shield_V2)让屏幕界面变得小菜一碟。[乔]编写了自己的声音和操纵杆代码，当然还有俄罗斯方块游戏本身，但如果没有[站在巨人](https://en.wikipedia.org/wiki/Standing_on_the_shoulders_of_giants)的肩膀上，这将远远超过几周的工作。查看[joo]的 Github 的[项目代码](https://github.com/vilaca/Handheld-Color-Console)，休息后请继续关注我们的演示视频和其他一些我们最喜欢的 Arduino 游戏技巧。

[https://www.youtube.com/embed/ycriUQhm9pg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ycriUQhm9pg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

现在，我们已经在这里看到了[大量](http://hackaday.com/2014/02/27/gamebuino-a-handheld-arduino-gaming-console-ready-for-prime-time/)基于 Arduino 的[游戏](http://hackaday.com/2013/11/28/8-bit-video-game-is-best-of-retro-gaming-on-a-shoestring-budget/)平台[，它们的范围从](https://hackaday.io/project/2219-arduino-game-console-the-blueokiris-gameduino)[简单的黑白](http://hackaday.com/2010/10/24/hackvision-is-build-your-own-retro-game/)到 [Gameduino](http://excamera.com/sphinx/gameduino/) 的花哨功能，Gameduino 将 FPGA 固定在你的 Arduino 上，以实现精灵、令人敬畏的声音和 VGA 输出。但是简单和易懂在我们心中也有一席之地，而[joo]的设备和代码已经明确地做到了这一点。

如果你准备将你的 Arduino 技能提升到闪烁的 led 之外，[joo]的游戏项目应该在你的阅读/构建清单上。我们迫不及待地想看到突破。

**后记:**【joo】完成了他的 Arduino [突围赛](https://github.com/vilaca/Handheld-Color-Console/tree/master/ArduinoBreakout)，还上传了一段视频。游戏性看起来不可思议。好光滑！

[https://www.youtube.com/embed/RhVOQ9A0XP8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/RhVOQ9A0XP8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)