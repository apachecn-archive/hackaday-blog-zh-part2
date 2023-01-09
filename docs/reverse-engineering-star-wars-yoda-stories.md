# 逆向工程星球大战:尤达故事

> 原文：<https://hackaday.com/2014/10/08/reverse-engineering-star-wars-yoda-stories/>

《星球大战:尤达故事》于 1997 年由卢卡斯艺术公司发行，评论界反响平平。正如 IGN 所说，“就像《幽灵的威胁》所证明的那样，只是因为它是《星球大战》并不意味着它是好的。”这并没有阻止扎克玩这个游戏，几年后，他对游戏的逆向工程产生了兴趣。

[扎克]的《星球大战:尤达故事》的[逆向工程](http://www.zachtronics.com/yoda-stories/) ( [谷歌缓存](http://webcache.googleusercontent.com/search?q=cache:http://www.zachtronics.com/yoda-stories/))查看游戏的数据文件。这个二进制文件由游戏在运行时解析，以提取音效、精灵和贴图。也许最著名的游戏数据文件类型是 Doom 的 [WAD 文件](http://en.wikipedia.org/wiki/Doom_WAD)，它有来自第三方的专门构建的编辑程序。

快速浏览了一下 [HxD](http://mh-nexus.de/en/hxd/) 中的数据文件后，【Zach】开始用 C#编写脚本来提取数据文件的不同部分。一旦找到这些部分，就可以使用更多的代码来应用调色板并生成位图。

最后，[扎克]设法得到了几千份游戏数据。他发现了一些有趣的东西，比如他在他的 mod 中替换了 X-Wing 的跑车。Lucasarts 早期游戏 *Indiana Jones 和他的桌面冒险*的引擎应该非常相似，一旦我们找到 Mac 安装盘和 ResEdit 的副本，我们就会在 Hackaday.io 上发布一些东西。