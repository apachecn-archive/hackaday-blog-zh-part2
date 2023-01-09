# SingLock 保护你的贵重物品免受害羞的人

> 原文：<https://hackaday.com/2014/12/17/singlock-protects-your-valuables-from-shy-people/>

两名康奈尔大学的学生设计了他们自己的[多因素认证系统](http://people.ece.cornell.edu/land/courses/ece4760/FinalProjects/f2014/aaw39_sh833/index.html "SingLock")。该系统使用 PIN 结合某种形式的语音识别来验证用户。然而，他们的系统并不像说口令那么简单。相反，你必须对着锁唱正确的音调。

该系统在 ATMEL MEGA1284P 上运行。这种芯片还不够复杂，无法轻易识别真实的人类语言。该团队决定将精力集中在探测音高上。结果是一把锁，要求你唱出完美的音高序列。我们会担心攻击者偷听并试图自己唱出音调，但是团队有一些机制来防止这种攻击。首先，系统还需要有效的 PIN。攻击者不能简单地通过在拐角处收听来推断出您的 PIN。第二，系统还维护用户的特定语音签名。

项目页面更深入地探究了系统如何工作背后的数学理论。如果你是数学或音频极客，这本书值得一读。请观看下面的视频进行演示。

[https://www.youtube.com/embed/3QbT2-mdAIQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/3QbT2-mdAIQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)