# 侵入 CSRF 的贝宝账户

> 原文：<https://hackaday.com/2014/12/04/hacking-paypal-accounts-with-csrf/>

自计算的早期以来，计算机安全行业已经发生了许多积极的变化。大型科技公司似乎正在流行的一件事是臭虫奖励计划。PayPal 提供了这样一个项目，Yasser 决定参与进来，看看他是否能找到任何有趣的漏洞。他的好奇心得到了巨大的回报。

Paypal 是支付处理领域的巨头，但这并不意味着他们没有缺陷。有时候目标越大，越难发现问题。[Yasser]想要试验跨站点请求伪造攻击。这种类型的攻击通常需要攻击者诱骗受害者点击恶意链接。然后，该链接将冒充受害者并代表受害者发出请求。只有当受害者登录到目标网站时，这才有可能。

贝宝有适当的保护机制来防止这种事情，但[亚西尔]发现了一个漏洞。当用户登录提出请求时，PayPal 会给他们一个认证令牌。这个令牌应该只对一个用户和一个请求有效。通过实验，[Yasser]发现了一种获得“万能钥匙”认证令牌的方法。攻击者可以尝试在没有首先登录任何 PayPal 账户的情况下发起支付转账。一旦尝试转账，PayPal 将要求用户进行身份验证。这个过程产生一个 auth token，它显然适用于来自任何用户的多个请求。这使得认证令牌几乎完全无效。

一旦攻击者拥有“通用身份验证令牌”，他就可以诱骗受害者访问恶意网页。如果用户当时登录了他们的 PayPal 帐户，攻击者的网页可以使用通用身份验证令牌来欺骗受害者的计算机发出许多不同的 PayPal 请求。示例包括向帐户添加电子邮件地址、更改安全问题的答案等等。所有这些都可以通过欺骗用户点击一个链接来完成。挺吓人的。

[亚西尔]当然要对他的揭露负责。他向 PayPal 报告了这个漏洞，并报告说这个漏洞很快就被修复了。看到像 PayPal 这样的大公司提倡负责任的披露并给予奖励，而不是打电话给律师，这总是很棒的。请务必观看下面的视频演示。

[https://www.youtube.com/embed/KoFFayw58ZQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/KoFFayw58ZQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [Reddit](http://www.reddit.com/r/netsec/comments/2o6ka5/hacking_paypal_accounts_with_one_click_max_paypal/ "Reddit.com")