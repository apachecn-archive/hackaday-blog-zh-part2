# 黑掉一个 20 美元的无线智能插头

> 原文：<https://hackaday.com/2014/11/13/hacking-a-20-wifi-smart-plug/>

Kankun 智能插头是一种廉价的设备，可以通过 wifi 开关插座。智能插头只能与设备自带的 Android 或 IOS 应用程序配合使用，这限制了它在打开和关闭手机上的功能。

为了让这个设备更有用，【LinuxGeek】用 *nmap* 探测了这个设备，[发现它运行 OpenWRT](http://www.htlinux.com/kankun-runs-on-openwrt-firmware/) 。在尝试了各种常见的默认密码后，他发现登录名是 *root/admin。*虽然[LinuxGeek]还没有嗅到这个协议，但是[其他人已经对它进行了更深入的研究](http://www.cnx-software.com/2014/07/28/kankun-kk-sp3-wi-fi-smart-socket-hacked-based-on-atheros-ar9331-running-openwrt/)。该插件显然使用 UDP 数据包与 Android 应用程序进行通信，但不幸的是，这些数据包被加密了。

他们没有破解协议，而是编写了从 CGI 脚本切换 GPIO 引脚的代码，并开发了一个小的 Windows 应用程序，该应用程序可以点击 CGI 脚本，以便从计算机进行简单的控制。还有一个 [Google+群](https://plus.google.com/communities/115308608951565782559)，在那里发布了更多关于这些插件的信息和一些其他的黑客攻击。售价 20 美元(来自全球速卖通),再加上一点黑客技术，这种智能插头可以很好地为家庭自动化系统增加无线控制。