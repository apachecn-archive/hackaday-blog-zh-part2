# 未经许可删除脸书专辑

> 原文：<https://hackaday.com/2015/02/15/deleting-facebook-albums-without-permission/>

[拉克斯曼]在脸书四处寻找安全漏洞。脸书运行着一个漏洞赏金计划，这意味着如果你能找到一个足够严重的漏洞，它可以为你赚得一大笔钱。[拉克斯曼]很快就找到了一个值得奖励的人。

graph API 是脸书应用程序读写脸书社交图的主要方式。许多应用程序都使用这个 API，但它能做的有一些限制。例如，API 无法删除用户的相册。至少，它不应该也能。[拉克斯曼]决定亲自验证这一说法。

他首先使用 graph explorer 访问令牌发送一个命令来删除他自己的一个相册。他的请求被拒绝了。应用程序没有正确的权限来执行该操作。看来脸书是对的，API 无法删除照片。[拉克斯曼]有另一个锦囊妙计。他注意到回复的措辞暗示其他应用程序将能够删除相册，所以他决定检查脸书移动应用程序。

他决定用不同的令牌发送相同的请求。这一次，他使用了来自脸书的令牌进行移动应用。这真的起作用了，结果他的相册被删除了。为了更进一步，[Laxman]发送了相同的请求，但将用户的 ID 改为他设置的受害者帐户。该请求被接受并顺利处理。这意味着[Laxman]可以有效地删除任何其他用户的相册，而无需该用户的同意。该漏洞首先需要[Laxman]具有查看相册的权限。

因为[拉克斯曼]是个好人，所以他把这个 bug 发给了脸书团队。他们花了不到一天的时间就解决了这个问题，并为此奖励了[拉克斯曼]12500 美元。被人欣赏总是好的。下面的视频展示了[Laxman]如何使用 Burp Suite 完成这次攻击。

[https://www.youtube.com/embed/trbriB_5qVA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/trbriB_5qVA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)