# 欺骗攻击通过利用社交登录机制窃取帐户

> 原文：<https://hackaday.com/2014/12/05/spoofedme-attack-steals-accounts-by-exploiting-social-login-mechanisms/>

我们都见过社交登录弹出框。你试图登录一些网站，却发现弹出框上写着“用脸书/推特/谷歌登录”。理论上这是个好主意。您可以使用一个凭证登录许多网站。这听起来很方便，但 IBM X-Force 的研究人员最近展示了这对您帐户的安全性有多么不利。更糟糕的是，如果提供了服务而你没有使用，你会更容易受到攻击。研究人员称他们的新发现为欺骗我。考虑到它允许攻击者欺骗易受攻击网站的用户并在该用户的帐户下登录，它的名称很恰当。

那么它是如何工作的呢？该漏洞利用了身份提供者(脸书/Twitter/etc)和“依赖网站”中的漏洞。依赖网站是用户试图使用其社交媒体帐户登录的任何网站。描述漏洞最简单的方法是浏览一个例子。开始了。

让我们假设你是一个攻击者，你想进入某个受害者的 Slashdot 帐户。如果你愿意，Slashdot 允许你在他们的系统内创建一个本地帐户，或者你可以使用你的 LinkedIn 帐户登录。你的受害者实际上没有 LinkedIn 账户，他们使用本地 Slashdot 账户。

攻击的第一步是使用受害者的电子邮件地址创建一个 LinkedIn 帐户。这必须是受害者用于本地 Slashdot 帐户的相同地址。这是第一个漏洞出现的地方。LinkedIn 需要允许创建帐户，而无需验证电子邮件地址是否属于您。

攻击的第二步现在是尝试使用您新创建的 LinkedIn 帐户登录 Slashdot。这就是第二个漏洞的来源。一些社交媒体服务会通过向 Slashdot 发送您的用户信息来验证您在 Slashdot 等网站上的身份。在这种情况下，关键信息是你的电子邮件地址。这是第三个漏洞。Slashdot 看到您的 LinkedIn 帐户与他们的一个本地用户有相同的电子邮件地址。Slashdot 假设 LinkedIn 已经验证了该帐户，并允许您(攻击者)以该用户的身份登录。你现在可以进入受害者的 Slashdot 账户了。在另一个场景中，Slashdot 可能会将两个凭证合并到一个帐户中。

关于这个黑客真正有趣的是，它甚至不是非常技术性。任何人都可以这样做。你所需要的只是受害者的电子邮件地址，你可以在各种社交媒体网站上试试看是否有用。更有趣的是，如果你不使用社交网站，你实际上更容易受到攻击。这种漏洞的一些真实例子是 LinkedIn 的社交登录服务、亚马逊的服务和 MYDIGIPASS.com 的服务。查看下面的演示视频。

[https://www.youtube.com/embed/kC0s3S00Dmk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/kC0s3S00Dmk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)