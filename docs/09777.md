# 设计日记:变容二极管调谐再生接收机

> 原文：<https://hackaday.com/2015/08/16/design-diary-varactor-tuned-regen-receiver/>

[QRP 盖金]喜欢建造再生接收器。如果你曾经建造过一个严重的，你知道有(至少)两个问题:一个是你需要一个可变电容器(现在很难找到)。另一个烦恼是，如果你覆盖很宽的频率范围，你可能需要不止一个线圈。

[【QRP 盖金】最新的无线电设计没有这些问题](http://theradioboard.com/rb/viewtopic.php?f=4&t=6418)。他用一个带单刀双掷开关的线圈来切换单个线圈。没有传统的主调谐电容。相反，1SV149 变容二极管提供无线电的主要调谐能力(二极管调谐范围为 35 至 500 pF)。

帖子提供了一个漂亮的设计和一个整洁的特百惠容器(嗯…至少外面是整洁的；里面是…最好留在特百惠里面)。更好的是，[QRP·盖金的]帖子详细描述了他是如何得到最终设计的，从想法开始，详细描述了最初的设计和他在这个过程中所做的改变。他还使用早期构建的数据来限制再生控制在宽频率范围内必须改变的程度，并详细说明了这如何改变设计。原型实际上没有计划的波段开关，但将覆盖 3 至 30 兆赫与正确的线圈。

当然还有更简单的再生接收器。然而，这种设计的复杂性以及设计师思维过程的细节使这成为一个有趣的中间周末项目。

[https://www.youtube.com/embed/LB8ISlB8bZE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/LB8ISlB8bZE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)