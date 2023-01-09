# 制作 9GHz 多普勒雷达

> 原文：<https://hackaday.com/2013/10/03/making-a-9ghz-doppler-radar/>

[卡勒]目前正在建造一个 FMCW 雷达，但由于他没有完成所有的部分，他决定同时建造一个 9GHZ 多普勒雷达。 [H 面喇叭天线](http://en.wikipedia.org/wiki/Horn_antenna)由黄铜片制成，焊接在一起。[卡勒]通过在发射器和天线之间插入一个[定向耦合器](http://en.wikipedia.org/wiki/Power_dividers_and_directional_couplers)并测量反射信号的强度(近似回波损耗)来检查发射器和天线之间的匹配。在 9Ghz 下，每秒 1 米的速度的多普勒频移约为 30Hz，因此他将雷达的输出信号连接到他的声卡上。

简单解释一下雷达使用的多普勒效应:如果你以给定的频率向移动的目标发送射频信号，反射信号的频率就会发生偏移。当一辆汽车鸣响警笛或喇叭接近、经过或远离观察者时，通常会听到这种声音。在接近时，接收频率较高(与发射频率相比),在经过时相同，在后退时较低。Hackaday 展示了大量使用这种效果的项目:一个[小型多普勒运动传感器](http://hackaday.com/2013/08/14/making-the-electronics-for-a-doppler-motion-sensor/)，[使用多普勒偏移的手势控制](http://hackaday.com/2013/06/10/gesture-control-uses-wifi-doppler-shift/)，[黑掉一把旧雷达枪](http://hackaday.com/2012/11/01/hacking-an-old-radar-gun-to-interface-with-a-laptop/)