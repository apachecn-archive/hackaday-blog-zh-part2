# 基本上，这是一个 ESP8266

> 原文：<https://hackaday.com/2015/08/29/basically-its-an-esp8266/>

在 Arduino 之前，有视差基础图章。这是一个用 BASIC 语言编写的 PCB 上易于使用的 PIC 芯片——本周早些时候，发表了一个关于这些卑微开端的故事。甚至在此之前，从 TRS-80 到 Commodore 64s，甚至牛郎星，大量的小型计算机主要由 BASIC 语言控制。BASIC 很容易在小型机器上运行，也很容易学习。老式的 BASICs 语言很难用来编写大型系统，但是许多小型计算机无论如何也不会运行非常大的程序。

ESP8266 不仅仅是微控制器的 WiFi 外设。这是它自己的小电脑。虽然运行“AT”固件、Lua 或自己对设备编程是很常见的，但是[您现在可以用 BASIC](http://www.esp8266basic.com/) 的一个版本来加载 beast。

当然，仅仅运行 BASIC 本身不会很有趣。真正的亮点是额外的关键字，允许控制设备的 WiFi 硬件，I/O 引脚和动态网页界面。您可以使用简化的 BASIC 语言及其扩展非常容易和快速地建立原型。

作为一个例子，这是项目主页上的一个例子:

```
cls
print "hello world"
let bla = "Test contents of textbox"
textbox bla
button "This is my button 1" [test1]
button "This is my button 2" [test2]
button Exit [TestExit]
wait
```

```
[test1]
print "You Clicked on 1"
print bla
wait
```

```
[test2]
print "You CLiked on 2"
let bla = "number 2 was clicked"
wait
```

```
[TestExit]
end
```

您可能会推断出第一个 wait 语句将生成一个带有文本框和三个按钮的 web 页面。单击按钮会导致代码的不同部分，要么生成新的网页，要么退出。像基本应该的那样简单。

关于如何将软件刷新到您的主板上，有明确的说明(但要准备好使用 Windows)。还有关于不使用多个空格的奇怪警告，所以显然该语言的解析器还需要一点工作。

如果你不喜欢 BASIC，并且你想要一个更直接的途径来编程 CPU T1，我们之前已经讨论过了。或者你可能想知道更多关于使用 Arduino IDE 支持模块的[。如果 BASIC 不是你的速度，你总是可以尝试 Lua，按照下面视频中的指示。](https://hackaday.com/2015/03/28/arduino-ide-support-for-the-esp8266/)

[https://www.youtube.com/embed/x-4LjjXB0f0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/x-4LjjXB0f0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)