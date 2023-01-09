# 用树莓皮控制的圣诞树装饰大厅

> 原文：<https://hackaday.com/2014/11/09/deck-the-halls-with-a-raspberry-pi-controlled-christmas-tree/>

当圣诞灯项目开始滚动时，你知道假日季节正在接近！[鱼鹰 22]在他的节日装饰上有了新进展，他用树莓皮控制的圣诞树灯光秀。是的，我们知道他可以用 Arduino 或 555 来完成，但 Raspi 是一个方便的平台。通过 WiFi 模块，可以远程更改代码。Raspberry Pi 的内置音频接口也可以轻松地将音乐与闪光灯同步，尽管我们可能会采用更高质量的 USB 音频接口。

[Osprey22 的] Raspberry Pi 正在运行自己定制的 python sequencer 软件。它接受一个 mp3 文件和一个序列文件作为输入，然后运行整个节目。当音乐不播放时，Pi 循环播放一组预定义的场景，每分钟改变一次。

硬件本身非常简单。Raspberry Pi 通过其 GPIO 接口控制 8 个固态继电器。8 串灯对于一般的树来说绰绰有余。[Osprey22]用一颗木头制成的星星点缀在树上，由一串 25 个 WS2801 RGB LED 像素照亮。

点击休息时间，查看[鱼鹰 22]树的行动！

[https://www.youtube.com/embed/kfC-06VcRJ8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/kfC-06VcRJ8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[通过指令]