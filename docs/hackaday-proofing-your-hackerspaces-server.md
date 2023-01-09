# 对你的黑客空间的服务器进行黑客日验证

> 原文：<https://hackaday.com/2012/10/06/hackaday-proofing-your-hackerspaces-server/>

![](img/8850464f81704338f5b88da3b4092f30.png "SERVER")

上个月，我们在 Hub City Labs 上发布了一篇关于在家自制 PCB 的教程。当时，Hub City 在一个会员慷慨提供的微型 vps 上托管他们的黑客空间网站。正如你所料，一群黑客读者把 Hub City Labs 的服务器变成了一堆熔渣，让他们的管理员头发变得更加灰白。他们的网站又恢复了，Hub City 提供了一个教程，教你如何保护你的服务器免受[攻击，被攻击，被删节，甚至被黑客攻击。](http://hubcitylabs.org/375-million-pageviews-for-15-a-month/)

最初几个小时的解决方案是将 Hub City Labs 的网站转移到一个亚马逊 EC2 实例上。从那以后，他们转向了 Debian EC2 实例，该实例能够处理 WordPress 站点每小时 50 万的页面浏览量。

这个惊人的功能需要很好的优化。WordPress 安装被设置为在每次页面加载时运行 cron 任务；如果你每分钟都要看到成千上万的点击，那就不好了。这些人将 define('DISABLE_WP_CRON '，true)添加到他们的 wp-config.php 文件中，并将所有后台任务(检查页面是否应该更新)设置为大约每分钟一次的固定时间表。随着 WordPress 缓存的增加，这些优化使每小时的页面浏览量从 1500 增加到 60000。

为了达到每小时 50 万的浏览量，EC2 实例加载了 [Varnish](https://www.varnish-cache.org/) ，这是一个前端缓存，可以真正加快速度。

结果——每月 15 美元的 3.75 亿次浏览量——可能超过了 Hub City Labs 的需求。然而，hackerspace 网站的性质——在 Hackaday、Slashdot 或 Reddit 发现你做了一些很酷的事情之前，负载很轻——意味着托管在可扩展的 EC2 实例上可能是一条出路。