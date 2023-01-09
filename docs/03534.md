# LED Strip Pong 作为 Arduino 屏蔽

> 原文：<https://hackaday.com/2013/07/06/led-strip-pong-as-an-arduino-shield/>

![led-pong-strip](img/3d152db47fa504a30a8ca8c5c928299e.png)

[Schuyler Sowa]一直在努力开发他自己版本的 LED 脱衣舞。我们会说他的工作确实得到了回报。这款游戏功能强大，功能丰富。

与最初的 Pong 视频游戏[不同，LED pong](http://hackaday.com/2012/08/22/one-dimensional-pong-is-a-great-use-for-led-strips/) 只有一个球运行的轴。当最后两个 LED 像素中的任何一个点亮时，如果按下条带末端的按钮，球将会反弹。为了增加难度调整，Schuyler 加入了一个可以改变速度的电位计。

游戏板是一米长的 LED 条，带有可单独寻址的像素。它的价格高达 28 美元，这是他在遇到基于 WS2801 的版本的问题后尝试的第二种产品(该版本通常以灯串的形式出现)。Arduino 板控制游戏，用 protoboard 制成的盾牌连接组件。除了两个用户按钮——它们是从计算机键盘上砍下来的——你会注意到一对七段显示器充当记分牌，还有一个 HD44780 字符 LCD 完善了用户界面。

[https://www.youtube.com/embed/uW_LPh4xO64?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/uW_LPh4xO64?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)