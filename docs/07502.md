# 非常大的触摸板适用于非常旧的计算机

> 原文：<https://hackaday.com/2014/11/06/very-large-touchpads-for-very-old-computers/>

很久以前，当我们大多数人还穿着尿布的时候，工程工作站有巨大的触摸屏，可以在 CAD 程序中绘图，绘图，以及 Wacom 平板电脑今天所做的一切。现在找到一个这样的触摸板是一件徒劳的事情，比找到它所连接的电脑更是如此，但[Daniel]找到了一种方法来重温那些大触摸板和旧电脑[与电阻式触摸屏和 MSX 电脑](https://translate.google.com/translate?sl=pt&tl=en&js=y&prev=_t&hl=en&ie=UTF-8&u=http%3A%2F%2Fhotbit.blogspot.com.br%2F2014%2F10%2Frecriando-uma-tabua-digitalizadora-para.html&edit-text=&act=url)(葡萄牙语，谷歌 [translatrix](https://translate.google.com/translate?sl=pt&tl=en&js=y&prev=_t&hl=en&ie=UTF-8&u=http%3A%2F%2Fhotbit.blogspot.com.br%2F2014%2F10%2Frecriando-uma-tabua-digitalizadora-para.html&edit-text=&act=url) )的日子。

[Daniel]正在使用通常用于显示器的触摸屏，通过 PIC16F micro 上的正确代码，触摸屏上的压力可以转换为 X 和 Y 坐标。在这种情况下，使用 PIC 是一个很好的选择:[使用 PIC](https://translate.google.com/translate?hl=en&sl=pt&tl=en&u=http%3A%2F%2Fdanjovic.blogspot.com.br%2F2014%2F10%2Ftelas-touchscreen-resistivas.html) 可以在一个 ADC 引脚上复用端口，使整个系统非常高效且易于校准。

之后，只需将微控制器的输出插入 MSX 的触摸板连接器，并编写几行 BASIC 代码在屏幕上画一个点。下面视频。

[https://www.youtube.com/embed/OHZBGVMgG8I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/OHZBGVMgG8I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)