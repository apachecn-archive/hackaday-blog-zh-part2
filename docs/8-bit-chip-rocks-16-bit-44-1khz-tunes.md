# 8 位芯片摇滚 16 位 44.1kHz 曲调

> 原文：<https://hackaday.com/2014/12/25/8-bit-chip-rocks-16-bit-44-1khz-tunes/>

我们心中有一个特殊的位置，可以容纳由您最喜爱的微控制器产生的芯片曲调。但是为什么就此打住呢？全功能音频是一个巨大的挑战，我们并不经常看到这种口径的例子。它[使用一个微控制器](http://people.ece.cornell.edu/land/courses/ece4760/FinalProjects/f2014/wz233/ECE%204760%20Final%20Report%20(HTML)/ECE%204760%20Stereo%20Player.html)输出 CD 质量的音频。

如何从 8 位微控制器中获得 16 位音频？我们给你一个提示:使用了两个引脚。无济于事？它来了:在这个芯片 ATmega1284 上使用了两个 8 位~~DAC~~PWM 输出。一个用于低八位，另一个处理高八位。两者结合使用精心计算的精密电阻值，结果超出你的想象。这是以 44077.135 的比特率制作的，与 44100Hz 的标准略有不同，但我们要求你的发烧友们说出其中的区别。wave 文件由 SD 卡提供，由芯片使用 Petit-FatFs 库读取。

这个项目有很多很棒的地方。首先，以周万成为例，任何人只要具备基本的微控制器技能，就能为安德鲁·杰克逊和华盛顿夫妇制作数字音频播放器。其次，那些具有中等 uC 技能水平的人会想要接受这个想法并为自己实现/调试它。[Wancheng]展示了如何使用 FFT 来衡量音频输出的质量。

如果你到今年还没搞清楚，这是康奈尔 ECE 4760 期末项目的又一个例子。向[[Bruce Land](http://hackaday.io/hacker/739-bruce-land)大声疾呼，感谢他们激发了令人敬畏的项目，并要求对项目进行广泛的文档记录，这本身就促进了对各个方面的深入了解。

[https://www.youtube.com/embed/CWsSt672qm0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/CWsSt672qm0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[通过 T0 黑客攻击。io]t1