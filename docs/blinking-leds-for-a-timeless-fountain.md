# 永恒喷泉的闪烁发光二极管

> 原文：<https://hackaday.com/2015/06/25/blinking-leds-for-a-timeless-fountain/>

我们以前见过一些这样的建筑，但是[Mathieu 的永恒喷泉](http://www.limpkin.fr/index.php?post/2015/06/30/A-Timeless-Fountain)的建筑质量很好地展示了机械技能，展示了闪烁的 led 灯的奇迹。

这个永恒的喷泉是我们之前见过的东西，这个想法实际上很简单:在滴水的水龙头旁边放一些发光二极管，根据水滴下落的速度对发光二极管进行计时，你就会得到一个频闪效果，使微小的水滴看起来悬浮在半空中。

像早期的建筑一样，[Mathieu]使用紫外线发光二极管，并用荧光素——一种紫外线活性染料——给水着色。led 安装在两个塔上，塔顶是一个小型低功率红外激光器和光电二极管。在 ATxmega16A4 上运行正确的代码，灯光会随着水滴的下落而及时闪烁，使水滴看起来好像悬浮在半空中。

快速闪烁 led 并不难。这个版本最大的问题是机制。这台机器的框架是用聚碳酸酯板加工而成的，很容易组装在一起。从水龙头获得持续的滴水有点困难。尝试了大约 15 次才把水龙头喷嘴的设计做对，但[Mathieu]最终选定了一个小的输出孔(约 0.5 毫米)和约 70 度的尖喷嘴角度。

[Mathieu]制作了一个视频，里面有一些悬浮的荧光球。你可以看看下面。在现实生活中，如果没有帧率问题，肯定会酷很多。

[https://www.youtube.com/embed/AOCZ0YukdeA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/AOCZ0YukdeA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)