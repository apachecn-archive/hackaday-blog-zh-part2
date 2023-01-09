# 在索尼电视上扎根

> 原文：<https://hackaday.com/2012/06/20/getting-root-on-a-sony-tv/>

索尼 Bravia 系列高清电视是一个很好的套件；它们是漂亮的显示器，通常有足够的输入用于最疯狂的家庭影院设置。这些电视也运行 Linux，但直到现在我们还没有看到任何利用这些显示器是壁挂式 Linux boxen 这一事实的东西。[Sam] [发送了一个漏洞](https://github.com/CFSworks/nimue)来修复任何 Bravia 电视——希望这是取代我们家庭媒体服务器的第一步。

该漏洞本身是由 Python 脚本初始化的常规缓冲区溢出。该脚本在任何带有 USB 端口的 Sony Bravia 上设置 Telnet 服务器，并提供完全的根用户访问。[Sam]能够在 USB 驱动器上运行 Debian 安装程序，所有的 Debian 程序都能正常运行。

如果您有一台 Bravia 想要在上面测试[Sam]的脚本，您需要一个用于电视的 USB 网络适配器和一个 Telnet 客户端来浏览电视的文件系统。现在还没有太多与 Bravia 相关的东西，但至少现在在电视上运行 XMBC 或其他媒体服务器是可能的。

如果有人想开始将 XMBC 移植到 Bravia 电视上，[Sam]说他非常愿意帮忙。我们不知道互联网上有任何 HDTV 改装社区，所以如果你是其中的一员，请在评论中发布链接。