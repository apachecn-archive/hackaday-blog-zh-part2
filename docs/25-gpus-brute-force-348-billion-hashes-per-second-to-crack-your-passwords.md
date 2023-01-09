# 25 个 GPU 强力每秒 3480 亿次哈希破解你的密码

> 原文：<https://hackaday.com/2012/12/06/25-gpus-brute-force-348-billion-hashes-per-second-to-crack-your-passwords/>

我们的理解是，视频游戏行业长期以来一直是新的更好的图形处理硬件的驱动力。但是他们不是这些进步的唯一资助者。正如我们之前所听到的，图形处理单元是唯一有资格快速处理加密哈希的(我们已经在比特币采矿中看到了这一点)。这个项目将 5 台服务器中的 [25 块 GPU 卡串在一起，组成一个超快速暴力攻击](http://securityledger.com/new-25-gpu-monster-devours-passwords-in-seconds/)。它的速度如此之快，以至于实际规格超出了我们的理解范围。一个人如何理解每秒 3480 亿次散列？

测试是在一组使用了 [LM](http://en.wikipedia.org/wiki/LM_hash) 和 [NTLM](http://en.wikipedia.org/wiki/NTLM) 协议的密码散列上进行的。NTLM 比 LM 更强，表现也更好，但这并不能说明什么。一个 8 个字符的 NTLM 密码将在 5.5 小时内失效，而一个 14 个字符的 LM 哈希只需要大约 6 分钟就能找到解决方案。当然，这种类型的硬件只有在您有密码散列本身的副本时才是好的。登录协议将在一定次数的尝试后被锁定，并采取措施来降低像这样的自动化系统的速度。

[via [Boing Boing](http://boingboing.net/2012/12/05/cracking-passwords-with-25-gpu.html)