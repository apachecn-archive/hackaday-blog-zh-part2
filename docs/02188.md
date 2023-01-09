# 由树莓皮制成的小 MAME 橱柜

> 原文：<https://hackaday.com/2012/11/26/tiny-mame-cabinet-built-from-raspberry-pi/>

已经有一段时间没有看到[Sprite_tm]凭空拉项目了，还没有看到他用一个树莓 Pi 做什么。所有的事情都会过去，最终[Sprite] [向世界展示了他的袖珍 MAME 机器](http://spritesmods.com/?art=rpi_arcade)。

构建使用了一个 Raspi 来处理所有 Linux-ey 和 MAME 的优点，但是[Sprite_tm]不想摆弄 HDMI 或模拟视频输出。相反，他选择使用一个只有 2.4 英寸宽的 [SPI 控制的 TFT 显示屏](http://spritesmods.com/?art=rpi_arcade&page=2)。这对于[Sprite]来说并不是一个新的黑客技术——今年早些时候，他发现了如何通过 GPIO 引脚[用杨桃](http://spritesmods.com/?art=spitft)连接这个显示器。

为了使他的柜子便于携带，[Sprite]选择使用旧手机电池和设计巧妙的充电电路。当电源连接到+5V 时，电池充电。当该电源被移除时，ATtiny85 向 Raspi 和显示器提供 5V 电源。

没有一个街机机柜是完整的，没有某种字幕，所以[Sprite] [使用了一个极其微小的 128×32 白色有机发光二极管](http://spritesmods.com/?art=rpi_arcade&page=6)来显示当前正在玩的游戏的标志。Raspi 中的一切都被设置为在游戏之间切换时完全无缝，自动配置当前所选游戏的控件和字幕。

你可以看看[雪碧]的迷你 MAME 在休息后直接进入泡泡漏，还有一些游戏镜头，最后切换到涅墨西斯。来自一个非常棒的制造商的非常棒的建筑。

[https://www.youtube.com/embed/5npkz0xY1fo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/5npkz0xY1fo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent) [https://www.youtube.com/embed/AzrvO8r8_pU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/AzrvO8r8_pU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)