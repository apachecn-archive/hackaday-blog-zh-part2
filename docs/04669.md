# 绕过希捷 ATA 安全锁

> 原文：<https://hackaday.com/2013/11/29/bypassing-seagate-ata-security-lock/>

这里有一个关于密码检索的常见故事:一个人安装了一台电脑，出于安全考虑，在他的希捷硬盘上设置了一个密码。几个月过去了，密码当然被忘记了。为了解决这个问题，硬盘在几个“计算机专家”之间来回移动，最终被放到了[blacklotus89]的工作台上。下面是他如何解决这个问题的。

接下来是几年前的黑客帖子。[blacklotus]最初发现[我们的一个帖子](http://hackaday.com/2011/02/18/hard-drive-password-recovery/)是关于硬盘上的 ATA 密码锁的。在下载了所需的工具后，他发现它只能在 WD 硬盘上运行，而不能在他桌子上毫无生气的 Seagate 上运行。[另一个黑客帖子](http://hackaday.com/2012/07/30/recovering-from-a-seagate-hdd-firmware-bug/)被证明更有前途。通过访问硬盘控制器的串行端口，[blacklotus]能够看到内存和缓冲区的前几行。

两个小时和两个 Python 脚本之后，[blacklotus]能够转储他的驱动器的内容。然后，他拿起另一个希捷驱动器，锁定它，转储它，并分析来自这个新锁定的驱动器的数据。他找到了自己的旧密码，并用同样的方法在以前无法破解的旧硬盘上寻找密码。原来旧硬盘的密码被设置为“0000”，这显然是一个非常安全的密码。

在浏览几个论坛时，[blacklotus]发现很多人在为同一个问题寻求帮助，很多回复说。我们不知道这个硬盘是不是你的，所以我们无法帮助你。看来那些代码迷不知道如何解锁硬盘，所以[blacklotus]把他所有的工具都放到了 GitHub 上。伟大的工作，一些事情并没有像[blacklotus]最初预期的那样以本周的黑客日[失败告终。](http://hackaday.com/tag/fail-of-the-week/)