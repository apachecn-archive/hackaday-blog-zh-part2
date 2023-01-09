# 在 Bose SoundTouch 中找到一个壳

> 原文：<https://hackaday.com/2014/09/30/finding-a-shell-in-a-bose-soundtouch/>

每个销售人员最喜欢的音响制造商 Bose 有一系列 Wi-Fi 连接系统。这是一个令人印象深刻的创新产品，能够连接到网络电台，潘多拉和存储在网络上其他地方的音乐库。这是一个非常棒的想法，因为它连接了一系列的网络服务，你只需要*知道*在某个地方有一个 Linux 外壳。[【莎拉】找到了](http://flarn2006.blogspot.com/2014/09/hacking-bose-soundtouch-and-its-linux.html)。

声音接触实际上很容易进入。唯一要做的实际工作是连接到端口 17000，打开远程服务，然后用 telnet 连接。用户名是 root。

端口 17000 上的 telnet 服务实际上非常有趣，我们猜测这就是 SoundTouch iOS 应用程序使用的所有魔法。[Sara]在 pastebin 上放了一个“帮助”命令列表[，看起来像是有切换 GPIOs 的命令，使用 Pandora 的命令，以及对蓝牙模块的引用。](http://pastebin.com/EXCQXmfY)

有趣的是，当[Sara]第一次怀疑这个盒子里可能有 Linux 时，她联系了 Bose 支持部门以获得任何信息。在 Bose 给她回邮件说这些信息本质上是专有的之前，她想出了自己的方法。