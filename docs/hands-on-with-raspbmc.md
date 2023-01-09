# 与 Raspbmc 一起动手

> 原文：<https://hackaday.com/2012/06/14/hands-on-with-raspbmc/>

[https://www.youtube.com/embed/0ps0THasUwA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/0ps0THasUwA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

你听说过树莓派吗？令人惊讶的是，它们开始慢慢流入成千上万的黑客手中，我们很幸运地得到了一个(二手的，因为我们没有及时赶上最初的预订)。我们一直渴望一个微小的嵌入式选项来运行 XBMC，这是我们见过的最好的机会之一。由[Sam Nazarko]创建的 Raspbmc 项目是为 XBMC 量身定制的，只需在邮件到达后几分钟就能让他看到树莓派。这正是我们所做的。

如果你熟悉向 SD 卡(或任何设备)写入图像，这是一个简单的过程。Raspbmc 作为一个单独的镜像文件发行，它启动 RPi 硬件，然后在下载和安装发行版的文件系统时将自身复制到 RAM。一旦卡亮了，就把它插进去，通电，然后等大约 20 分钟，直到 XBMC 出现在屏幕上。之后每次都是快速启动。

好消息是它起作用了。XBMC 运行得相当快，只是加载一些菜单时有一点滞后。使用我们熟悉的 confluence 皮肤时，我们感觉就像在家里一样，并且在设置视频库的 samba 共享时没有任何问题。唯一的问题是它不能播放我们手头的任何视频文件。一个都没有。所以我们下载了*大巴克兔*预告片。它也不会播放那个。这完全是一个编解码器问题。虽然 RPi 上使用的芯片能够对 MPEG2 视频进行硬件解码，但基金会并没有授权这种能力。所以它不能播放那种格式，句号。对于电影预告片，我们尝试了 OGG 格式，目前不支持，但 MOV 版本可以播放，完全 1080p 没有问题。

因此，结论是，如果你想找一个 RPi 来管理 XBMC，你应该等等。到目前为止，这个方案是有希望的。但是我们录的是 ATSC 的视频，都是 MPEG2。如果您使用 MakeMKV 在服务器上存储您的 DVD，那么它也使用 MPEG2。当然有选择转码一切。但是，如果你有其他 XBMC 前端可能无法播放替代编码，你要小心。