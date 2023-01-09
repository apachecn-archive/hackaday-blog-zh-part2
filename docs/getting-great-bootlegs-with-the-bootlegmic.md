# 用盗版音乐获得好的盗版音乐

> 原文：<https://hackaday.com/2012/05/21/getting-great-bootlegs-with-the-bootlegmic/>

去任何音乐会，演出，或地下室乐队练习，你会发现有人录制盗版。虽然这些现场录音有时质量相当高，但用手机录制的盗版音乐通常听起来很糟糕。开放音乐实验室的人有一个解决这些低质量录音的好办法，只需要几美元的零件。

这个项目叫做[盗版](http://www.openmusiclabs.com/projects/bootlegmic/)。这是对驻极体麦克风的简单改造——与手机和蓝牙耳机中的麦克风类型相同——可以在非常嘈杂的环境中进行高质量的录音。根据[开放音乐实验室 wiki](http://wiki.openmusiclabs.com/wiki/BootlegMic) 的说法，修改非常简单，只需在驻极体麦克风的 PCB 上切割几条迹线，然后焊接一个电容和几个电阻。

驻极体话筒包含一个小 JFET，用于放大来自话筒振膜的信号；特定的 JFET 由制造商选择，以确保麦克风具有正确的增益和响应。通常选择这些 JFETs 是希望有一个相对安静的环境，而试图录制一场音乐会只会导致大量失真。通过在 JFET 源和麦克风地之间放置一个电阻，可以降低这种失真。

该电路很容易焊接死插头风格，并应与大多数手机。开放音乐实验室的人能够让他们的麦克风在 iPhone 上工作，但他们仍在努力找出 Android 麦克风输入。有一个很棒的演示视频展示了音频质量的提高；休息之后你可以去看看。

[https://www.youtube.com/embed/72dNV0iFajQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/72dNV0iFajQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)