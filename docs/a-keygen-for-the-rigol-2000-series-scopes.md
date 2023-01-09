# Rigol 2000 系列示波器的钥匙

> 原文：<https://hackaday.com/2013/07/24/a-keygen-for-the-rigol-2000-series-scopes/>

几周前，我们注意到 Rigol 的 DS2000 系列示波器通过几个 USB 命令就可以轻松解锁。我们原本预计会开发一种小型微控制器设备，将这些位自动发送到示波器，我们从未想到这个工具黑客的最终版本会如此优雅。现在，只需一个序列号和一个很棒的加密技术，就可以[解锁 ds 2072 o’scope。](http://freneticrapport.blogspot.com/2013/07/raspberry-pi-rigol-ds2072-200mhz.html)

Rigol 的工程师们(上帝保佑他们)为 800 美元的 70MHz DS2072 和 1600 美元的 200MHz DS2202 使用了相同的硬件。两者之间的唯一区别是示波器内存中的一些位，如果你有正确的钥匙，这些位很容易被解锁。EEV 博客论坛上的一些人计算出了示波器加密的私钥，用户[【cybernet】写了一个 keygen](http://www.eevblog.com/forum/testgear/sniffing-the-rigol's-internal-i2c-bus/msg264876/#msg264876) 。

升级过程非常简单:获取您的 DS2072 的序列号，将其放入 keygen 中，并将生成的密钥输入到 scope 中。重启，你就有了一个半价买的 1600 美元的望远镜。