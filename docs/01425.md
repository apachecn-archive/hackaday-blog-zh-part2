# 在旧的 Mac ROMs 中发现复活节彩蛋

> 原文：<https://hackaday.com/2012/08/24/uncovering-easter-eggs-in-old-mac-roms/>

![](img/99515bf5378b7cde81b5bef5192d4380.png "pic")

你在上面看到的图片是从 20 世纪 80 年代末生产的 Macintosh SE 的 rom 中截取的。这张黑白照片一直埋藏在旧 Mac 电脑中，直到纽约电阻器公司的[Adam]和[Trammell]对这些旧 Mac 电脑的 rom 进行了逆向工程，发现了一些非常酷的复活节彩蛋。

[Adam]和[Trammell] [从旧电脑中倾倒 rom](http://www.nycresistor.com/2012/07/07/stick-a-straw-in-its-brain-and-suck-how-to-read-a-rom/)已经有一段时间了。他们的作案手法是在旧电脑上找到旧的 27C 系列 EPROMs，从他们舒适的家中撬出，把它们放在试验板上，然后连接 Arduino 克隆体将数据转储到电脑上。

最近，这些家伙在布鲁克林的路边发现了一台旧 Mac SE，并将它带到了纽约电阻器公司。他们已经知道图片藏在只读存储器里，但是他们想知道这些图片是如何储存的，储存在哪里。在仔细检查了转储 rom 生成的二进制文件后，[Adam]能够恢复隐藏在每台 Macintosh SE 中的三个映像。

苹果公司的员工——尤其是在 Apple II 和 68k Macs 令人兴奋的日子里——在他们电脑的 rom 中藏了不少复活节彩蛋。例如，Apple IIgs 将音频数据存储在 ROM 中，Macintosh Classic 将整个操作系统(系统 6.0.3)隐藏在机器的 ROM 中。

通过[使](http://blog.makezine.com/2012/08/21/rom-dumping-leads-to-discovery-of-25-year-old-easer-egg/)