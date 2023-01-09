# 比格犬代表游戏男孩，游戏男孩前进，NES，还有——是的——SNES

> 原文：<https://hackaday.com/2015/03/03/beaglesnes-for-game-boy-game-boy-advance-nes-and-yes-snes/>

到目前为止，Raspberry Pi 最常见的用途是将几十个模拟器放在 SD 卡上，然后就结束了。每个人都有起点，对吧？还有其他小型的、信用卡大小的 Linux 主板，而[Andrew]正在将 Raspi 的相同功能引入 BeagleBone Black 和 beagle board[with beagles nes](http://hackaday.io/project/3913-beaglesnes)，这是一个适用于所有 sane pre-N64 控制台的仿真器。

BeagleSNES 最开始是作为嵌入式系统设计的一个类项目，但是简单移植 SNES9X 的性能默认不是很好。[Andrew]最终破解了引导加载程序和内核，剖析了仿真器，并在三年的开发过程中慢慢地使它成为可能的最佳仿真器。

经过几个月的开发，[Andrew]最近发布了新版本的 BeagleSNES，它包括 OpenGL ES，通过 BeagleBone 的 PRU 提供原生游戏手柄支持，以及对所有旧的任天堂游戏机和便携式设备的支持。下面是视频演示。

[https://www.youtube.com/embed/NnWxf2hWFcw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/NnWxf2hWFcw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/jp7inzxFHCc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/jp7inzxFHCc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)