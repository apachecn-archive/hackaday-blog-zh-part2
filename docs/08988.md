# 覆盆子果酱——梅森罐中的 BitTorrent 同步客户端

> 原文：<https://hackaday.com/2015/05/09/raspberry-preserve-a-bittorrent-sync-client-in-a-mason-jar/>

[Matt Reed]使用一些现成的部件，构建了一个基于 Raspberry-Pi 的 BitTorrent 同步客户端来帮助备份文件。让它脱颖而出的是使用梅森罐作为外壳和漂亮的构建完成的想法。梅森罐长期以来被用来保存食物。[ [马特](http://twitter.com/mcreed)想用梅森罐来帮助保存家庭记忆。

基本上，他只是在一个装有 LED 灯的罐子里塞了一个树莓派，然后放上 BitTorrent Sync。他从一块漂亮的方形木头开始，把盖子盖在上面。钻孔是为了固定四个 led 和人造水晶抽屉拉钮。Pi 连接到电源和以太网，LED 连接好。软件非常简单——只需在树莓 Pi 上安装 [BitTorrent Sync](https://www.getsync.com/) 。他写了一个 [Node.js 脚本](https://github.com/mcreed/raspberry-preserve)来不断检查 BitTorrent Sync 是否正在传输任何数据，如果是，闪烁 LED，这样看起来很酷。如果没有数据正在传输，LED 只会发出稳定的红光。一旦插上电源并连接到互联网，任何照片或视频(或任何文件)都会被放在他的任何设备上一个名为“Preserve”的特殊文件夹中，并被同步和复制到“Raspberry Preserve”中，为子孙后代保留下来。