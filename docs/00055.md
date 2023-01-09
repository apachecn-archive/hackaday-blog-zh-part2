# 想要一个两人自毁按钮，但厌倦了讨厌的微控制器？

> 原文：<https://hackaday.com/2012/04/08/want-a-two-person-self-destruct-button-but-tired-of-pesky-microcontrollers/>

![](img/954751ec3ad5f495624475b9c4a64cbf.png "self destruct")

我们都知道我们珍贵的巡洋舰/战舰/资产不能落入坏人之手，还有什么比在设计中加入自毁按钮更好的方法来确保信息安全呢？虽然总的前提是足够简单的唯一真正的方法，以确保一些疯狂的太空病毒不能感染你的船长，并迫使他摧毁你的船是增加一个两个按钮的安全系统！等等，如果是电脑病毒呢？！嗯,[安德里亚]用这个[双手控制](http://www.instructables.com/id/Two-hand-control/)开关把它盖住了。我们猜测你也可以使用这个方案来打开一个危险的设备，因为它迫使操作员从机器上移开双手来操作按钮，但是这有什么戏剧性呢？

使用分压器和电容的组合来激活晶体管，一个激活 555 定时器，另一个在半秒左右后禁用按钮输入，从而对按钮进行计时。由于全是电阻电容时序，您的电路可能只需要一点调整(或精密元件)就能一切正常。使用两个人来触发输出有一点问题，因为第二个按钮实际上直接操作输出继电器。如果按住第二个按钮，它只会在计时器的输出被触发之前保持活动，但如果你的副手临阵退缩，在核心变热之前释放了按钮，那么，你将会尴尬的慢跑到逃生舱。

在跳伞后检查视频，看看[安德里亚]摆弄开关。

[https://www.youtube.com/embed/G9uHNrIsJvA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/G9uHNrIsJvA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)