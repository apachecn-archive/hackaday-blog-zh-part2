# 使用 ATtiny13 的伪随机闪烁南瓜灯 LED

> 原文：<https://hackaday.com/2013/10/22/pseudo-random-flickering-jack-o-lantern-led-using-attiny13/>

[![Pseudo_Random_Flicker_ATtiny13](img/2bcca00c3b758262ae9337b282dd3291.png)](http://hackaday.com/wp-content/uploads/2013/10/pseudo_random_flicker_attiny13.jpg)

是时候让那些空心南瓜灯为万圣节闪烁了。如果你不想在这个万圣节使用蜡烛或购买南瓜灯，你可以像[约翰内斯·鲍尔]一样，编写自己的[伪随机闪烁超亮 LED](http://www.youtube.com/watch?v=jX4KXbO8Q5g) 。他的妻子希望他们的南瓜今年被照亮，他知道用 Arduino 很容易做到，但对于这样一个简单的项目来说，这将是大材小用。另外，他没有 arduino。[Johannes]使用很少的组件；4 节稍微耗尽的 AA 电池，一个超亮的 LED，680 欧姆的电阻和一个 8 针 ATtiny13 上的一点自定义代码。该电路对于南瓜灯来说确实很棒，但他的视频更像是一个关于为 8 位伪随机 LED 闪烁编码的[线性同余发生器](http://en.wikipedia.org/wiki/Linear_congruential_generator) (LCG)的教程。

代码很短，可以从 YouTube 视频中找到。[Johannes]使用 avr-gcc 进行编译，并且已经[打包了他的代码和构建脚本供下载](http://johannes-bauer.com/flicker-0.01.tar.gz)。可以使用 avrdude 或 AVR Studio 将十六进制文件闪存到芯片上。如果你身边有任何 ATtiny13s，你应该及时拼凑出这个程序来模拟南瓜蜡烛的真实外观，而没有真实火焰的麻烦和危险。

如果你想要更亮的东西，但仍然像蜡烛一样闪烁，那么看看“[闪烁的南瓜灯](http://hackaday.com/2013/10/01/flickering-pumpkin-lanterns/)”，它使用 LED 茶灯的信号为一些 12 V 灯供电。

休息后请继续观看[约翰内斯·鲍尔的]视频。

[https://www.youtube.com/embed/jX4KXbO8Q5g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/jX4KXbO8Q5g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)