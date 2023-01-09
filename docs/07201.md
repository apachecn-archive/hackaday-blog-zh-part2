# 用铅笔和纸挖掘比特币

> 原文：<https://hackaday.com/2014/09/29/mining-bitcoins-with-pencil-and-paper/>

目前，有数千台电脑连接到互联网，尽职尽责地计算 SHA-256 哈希，并将结果发送给比特币网络上的其他同行。在这个网络中有着巨大的计算能力，但是[【Ken】正在用铅笔和纸](http://www.righto.com/2014/09/mining-bitcoin-with-pencil-and-paper.html)做这件事。手工计算并不难，但它确实需要大量的时间；[Ken]每天可以计算大约三分之二的哈希。

用于比特币的 SHA-256 哈希函数手工计算起来并不困难。但问题是，它接受一个 64 字节的值，通过算法发送，并重复 64 次。有一些 32 位的加法，但剩下的工作只是在一组三位中选择多数值，旋转位，并执行 mod 2。

完成一轮阿沙-256 哈希需要[Ken]16 分 45 秒。计算散列需要 64 个步骤，这意味着一个散列需要大约 18 个小时才能完成。由于比特币使用双 SHA-256 算法，在一个完整的比特币块上进行计算并手动提交给网络需要两天的时间。如果你只是每天朝九晚五地做这件事，这是一整周的工作。

只是为了好玩，[Ken]试图弄清楚他头骨里储存的比特币挖矿钻机到底有多节能。他不能靠电力生活，但油炸圈饼是一种廉价的卡路里来源，每 200 千卡约 0.23 美元。假设代谢率为 1500 千卡/天，这意味着他的能量消耗约为 ASIC 矿工的 67 万亿倍。

下面视频。

[https://www.youtube.com/embed/y3dqhixzGVo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/y3dqhixzGVo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)