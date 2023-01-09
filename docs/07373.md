# 使用 Android 控制翻盘显示器

> 原文：<https://hackaday.com/2014/10/20/controlling-a-flip-disc-display-using-android/>

当大多数人看到机电显示器时，他们会被吸引住；虽然你很难找到便宜的翻盖显示器，但你仍然可以很容易地买到翻盖显示器！这就是[斯科特]所做的，他一直在摆弄他的和[建立一个系统，通过他的 Android 手机来控制它。](http://www.scottcutler.net/projects/flipdots/flipdots.html)

他从波兰一家名为 [Alfa-Zeta](http://www.flipdots.com/flip-dot-boards-xy5-14x28.html#.VEV__vnF8Xw) 的公司获得了这款显示器，这家公司自 1988 年以来一直在制造电磁显示器。没有提到价格，但它看起来像一些非常可怕的硬件。电磁显示器的美妙之处在于，它们在空闲状态下不消耗任何电力，这使得它们比几乎任何其他显示技术都要高效得多——更不用说在任何照明条件下都有完美的对比度了！

它们通过使用永久磁铁、电磁铁和一种可以保持磁化的材料来工作。电磁体的一个短脉冲导致圆盘翻转到第二个位置，然后由于永磁体的作用，圆盘将保持在原位——不再需要电磁体。

显示器配有所有必要的硬件来驱动电磁铁，并与微控制器接口。但是，它使用 RS-485 标准，大多数其他微控制器本身并不支持该标准。[Scott 的]使用的 Arduino 确实有 RS-485 屏蔽，但他决定挑战自己，建立一个电路来自己驱动它们！

如果你想尝试类似的东西，所有的信息都在他的博客上。一旦他将它与 Arduino 接口，就只需编写一个 Android 应用程序，通过蓝牙传输对显示器的控制。看一看:

[https://www.youtube.com/embed/bMWYmIQlA2c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/bMWYmIQlA2c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

给你来点慢动作:

[https://www.youtube.com/embed/WSfdnoRUO3I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/WSfdnoRUO3I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

如果分割盘对你来说不够机械，你可以尝试[制作自己的分割盘展示……](http://hackaday.com/2014/10/04/split-flap-display-if-cant-find-it-built-it/)