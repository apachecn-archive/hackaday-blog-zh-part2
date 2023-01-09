# 轻松将您的树莓皮变成调频发射机

> 原文：<https://hackaday.com/2014/06/15/easily-turn-your-raspberry-pi-into-an-fm-transmitter/>

你有没有想过成为自己的电台 DJ？[Kevin]用他的 Raspberry Pi[FM 发射程序](http://techzei.com/how-to-build-a-raspberry-pi-radio-transmitter/ "Fm Transmitter program")让它变得前所未有的简单。该程序是用 c 语言编写的。[Kevin]已经提供了源代码和编译后的二进制文件。

PIFM 允许您加载任何音频文件并指定传输频率。然后，程序将使用 PWM 通过 Pi 的 GPIO4 引脚调制音频样本。[Kevin]声称 RasPi 本身只能传输大约 10 厘米的距离。他说用跳线制作一个简单的天线可以将距离增加到 100 米左右。你所要做的就是将电线连接到 GPIO4 引脚，以大幅增加范围。

这种发射机的合法性因地而异，所以在你用规定的频率发射音频之前，一定要检查你当地的法规。如果你对这种东西感兴趣，你可能想调查一下业余无线电。不全是莫尔斯电码和老古董。有些人声称这是黑客的天堂。

[via [Reddit](http://www.reddit.com/r/raspberry_pi/comments/2844k1/how_to_build_a_fm_radio_with_raspberry_pi_5_min/ "Reddit.com")