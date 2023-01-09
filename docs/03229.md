# Pebble Watch Hack 使其成为家庭自动化控制器

> 原文：<https://hackaday.com/2013/05/03/pebble-watch-hack-makes-it-a-home-automation-controller/>

[Enrico]热爱他的 Pebble 手表，最近有机会探索用于定制其功能的代码包。事实证明这真的很容易操作，所以他着手[将 Pebble 手表变成一个家庭自动化控制器](http://makr.co/blog/pebble-home-automation/)(死链；[互联网档案馆](http://web.archive.org/web/20130504022802/http://makr.co/blog/pebble-home-automation/)。

到目前为止，他的实验中使用的两个硬件如上图所示。手表本身充当控制器，与背景中的以太网中继板交互。这款手表通过蓝牙进行通信，但你不必了解太多，因为你可以从[存储库](https://github.com/Hexxeh/libpebble)获得示例文件。考虑到通信问题，他需要一个菜单系统来访问手表上的命令。他没有编写自己的代码，而是在内置的音乐菜单中加入了一个播放列表。这使他能够再次打开和关闭继电器，就像他在播放或暂停音轨一样。休息之后看看它的实际效果。

[https://www.youtube.com/embed/G1TKKiCGTDs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/G1TKKiCGTDs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)