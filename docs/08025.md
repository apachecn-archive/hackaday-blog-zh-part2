# 绕过损坏的 SIP ALG 实现

> 原文：<https://hackaday.com/2015/01/11/bypassing-broken-sip-alg-implementations/>

SIP 协议通常用于 IP 电话通信。不幸的是，它因 NAT 穿越问题而臭名昭著。甚至一些主要供应商似乎也不能正确理解。[Stephen]他的 Cisco WRVS4400N 路由器出现了这个问题。经过一点故障排除，他能够想出一个其他人可能会发现有用的[解决方法](http://technogrumble.blogspot.com/2013/01/router-breaks-sip-work-around-it.html "Bypassing SIP ALG")。

该路由器内置了 SIP [ALG](http://en.wikipedia.org/wiki/Application-level_gateway "Application lLevel gateway") 功能，但它就是不工作。[Stephen]试图将 SIP 通信从一部电话路由到路由器后面的一个[星号 PBX](http://hackaday.com/2012/08/22/building-a-pbx-setup-around-the-raspberry-pi/ "Asterisk PBX on a Pi") 系统。无论启用还是禁用 SIP ALG，路由器都无法正确处理这些数据包。

[Stephen]首先尝试将外部 VOIP 电话上的 SIP 端口从默认的 5060 更改为其他端口。然后，他在路由器上设置端口转发到星号框，将流量转发到原始端口上的星号系统。这种方法有点奏效。电话会接通，但大约 20 秒后会掉线。

[Stephen]唯一能做的事情就是使用“bindport”指令更改 Asterisk 的 sip.conf 文件中的 SIP 端口。他将其更改为某个随机的未使用的高端口号。然后，他在路由器上设置端口转发，将该端口上的传入 UDP 数据包转发到 Asterisk 系统。这工作得很好，但是现在路由器后面的所有原始电话都停止工作了，因为它们被配置为使用默认端口 5060。

[Stephen]没有重新配置组织中的所有电话，而是对 Asterisk 系统进行了一项更改。他设置了一个 iptables 规则，将 UDP 端口 5060 上的所有传入流量转发到新的 SIP 端口。现在，整个组织中所有的电话都在进行最小的改动。仅仅因为路由器不能正确处理 SIP 就要经历很多麻烦，但是它完成了任务。