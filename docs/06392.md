# 生根巢恒温器

> 原文：<https://hackaday.com/2014/06/24/rooting-the-nest-thermostat/>

几个月前，谷歌购买了一个价值 32 亿美元的恒温器，希望它能为每个家庭的智能设备铺平道路。Nest 恒温器本身实际上非常酷——它运行 Linux，具有相当强大的 CPU，并为一些潜在的酷应用程序添加了 WiFi。[也可以在一分钟之内扎根](http://blog.gtvhacker.com/2014/google-nest-exploiting-dfu-for-root/)，

正如[cj]解释的那样，Nest 内部的 CPU 有一个设备固件更新模式，通常用于 Nest 工厂内部的测试。这种 DFU 模式也可以用来修改设备，没有任何限制。

通过一个简单的 shell 脚本，[cj]将 Nest 插入他的笔记本电脑的 USB 端口，将设备置于 DFU 模式，并上传一个两阶段 booloader，以实现对 Linux 驱动的恒温器的完全控制。

另外，shell 脚本还安装了一个 SSH 服务器，并支持一个反向 SSH 连接来绕过大多数防火墙。这使得任何人都可以远程控制 Nest 恒温器，这是 Nest 的一个很好的补充，它不依赖于 iPhone 应用程序或云服务来远程控制你的互联网恒温器。

下面是生根过程的视频。

[https://www.youtube.com/embed/H3tmvpi4YR0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/H3tmvpi4YR0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)