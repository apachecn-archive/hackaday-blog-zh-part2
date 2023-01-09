# 用于 CMOS 合成器的时钟 8 位随机码发生器

> 原文：<https://hackaday.com/2015/02/11/clocked-8-bit-random-pattern-generator-for-a-cmos-synth/>

在处理音乐时，随机噪声发生器非常方便，使用微控制器制作一个随机噪声发生器可能非常简单。因此，当有人来用一些模拟和数字器件构建它时，感觉很好。[酸波旁]建立了他的[时钟 8 位随机模式发生器的 CMOS 合成器](https://acidbourbon.wordpress.com/2015/02/07/clocked-8-bit-random-pattern-generator-for-cmos-synth/)灵感和动力来自最近的文章[逻辑噪声:甜蜜，甜蜜的振荡器声音](http://hackaday.com/2015/02/04/logic-noise-sweet-sweet-oscillator-sounds/)【埃利奥特·威廉姆斯】。它的 8 位输出可以用作 DIY CMOS 合成器的随机序列发生器。
该图形发生器适合与 4051 8 通道模拟多路复用器结合使用。但它本身听起来很有趣(最好在立体声中欣赏，休息后查看视频)。在制造了一些 CMOS 合成器电路之后，[酸波旁]继续制造一些序列发生器和多路复用器，这使他能够设计这种可以用时钟信号门控的随机模式发生器。

基本原理非常简单——产生噪声，将其放大，施加时钟以获得门控噪声输出。基于他必须处理的约束条件，他对各个部分的设计选择得到了很好的解释。一切都需要 5V 工作，但他的噪声发生器电路需要 12V 工作。他选择使用一个电荷泵来产生-5V 电压，从而得到一个 10V 的电源，这虽然勉强够用，但还是起作用了。升压调节器可能会更好地产生 12V，但也许他已经有 ICL7660 电荷泵 IC 躺在他的零件箱里。电路的其余部分使用标准的 CMOS/TTL 器件，而[acidbourbon]提供了所有的设计文件，看起来像一个整洁的单面 PCB，可以使用[墨粉转移方法](http://hackaday.com/?s=toner+transfer+method)轻松制作。

下面视频。

[https://www.youtube.com/embed/CAIM0nA8JoA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/CAIM0nA8JoA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)