# Shinewave Gamecube 控制器对 Smash 兄弟的反应

> 原文：<https://hackaday.com/2015/08/02/shinewave-gamecube-controller-is-shiny/>

[加勒特·格林伍德]扮演粉碎兄弟，显然相当严重。以至于他需要用五个新像素来修改他的控制器[,这样它就可以根据他在控制器上弹奏的组合键来闪烁不同颜色的动画；当然，是根据他最喜欢的角色的动作颜色量身定做的。](http://www.electricexploits.net/shinewave/)

所有这一切都发生在 85 岁的大脑身上，我们发现这是相当雄心勃勃的。事实上，[Garrett]开始认为他可以简单地将控制器的每个输入直接读取到整个事情的核心微控制器中，但随后计算出有多少根导线，并查看他有多少个空闲引脚(六个)，并想出了一个更好的解决方案。

[Garrett]的例程读取 Gamecube 控制器用来发送回控制台的单行代码。[协议很好理解](http://www.int03.co.uk/crema/hardware/gamecube/gc-control.htm)，用长短和长短信号进行比特编码。唯一的诀窍是每一位在 4 微秒内发送，所以解码程序必须相当快。为了使它工作，他必须做相当多的工作。休息之后，我们会有更多的内容和演示视频。

[https://www.youtube.com/embed/1U4EOI_aFdc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/1U4EOI_aFdc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[加勒特]目前的职位只涵盖了硬件和使用的东西。我们屏住呼吸等待软件报告。要完善自己的哨子，请查看[【Garrett】的 Github](https://github.com/GGreenwood/BlinkCube) 并自己浏览代码。我们粗略通读了以下要点:

*   Gamecube 协议在汇编程序中编写的[中断程序中处理](https://github.com/GGreenwood/Shinewave/blob/master/ANA_COMP.S)
*   使用轻量级微控制器线程的 [Protothreads](http://dunkels.com/adam/pt/) 库处理动画
*   一般性感的编码，包括一个漂亮的[手工构建的 Makefile](https://github.com/GGreenwood/Shinewave/blob/master/Makefile) (我们喜欢的方式)

我们不知道你有多少空闲空间，[加勒特]，但我们认为如果你能把一个串行引导加载程序挤进芯片会很酷，这样你就可以更容易地更新它，而不用打开和关闭外壳。TinySafeBoot 或(老派)【彼得·丹内格/《丹尼》】的[快速启动](http://www.avrfreaks.net/projects/fast-tiny-mega-uart-bootloader?module=Freaks%20Academy&func=viewItem&item_id=1008&item_type=project)可能对你有好处。

哦，加勒特给我们发邮件说，他正在寻找一家塑料公司来生产像他这样的 Gamecube 控制器的透明背面，如果他能找到的话，他正在考虑经营一个 Kickstarter。保持警惕。

感谢[Bigjosh2]的提示！