# 将耳机插孔用作 UART

> 原文：<https://hackaday.com/2014/11/04/using-a-headphone-jack-as-a-uart/>

我们以前见过音频端口被用来在计算机和微控制器之间建立通信通道，[但没有一个像这个](http://forum.espruino.com/conversations/257732/)这么巧妙。[Gordon]正在使用平板电脑上运行的网页向微控制器发送 Javascript，整个程序在微控制器中被解释。

[Gordon]正在使用 Espruino Pico，这是一款现在已经在 Kickstarter 上发布的板[。这个小小的板是围绕一个 javascript 解释器构建的，允许动态地编写和更新代码，而不需要使用引导加载器。](http://hackaday.com/2014/10/29/espruino-pico-javascript-on-a-usb-stick/)

这种技术可以扩展到在微控制器和计算机之间提供双向通信。在 Github 项目中，【Gordon】使用 TRRS 插孔上的麦克风引脚向计算机发送数据。它还需要两个电阻，但除此之外，它就像单向通信设置一样简单。

[Gordon]将该程序的几个演示放在一起，其中一个将根据网页上的输入改变一些 RGB LEDs 的颜色。

[https://www.youtube.com/embed/BQDZNFXygrM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/BQDZNFXygrM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/IP7e5KJGVnM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/IP7e5KJGVnM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)