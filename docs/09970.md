# FCC 引入禁止修改 WiFi 路由器固件的规则

> 原文：<https://hackaday.com/2015/08/31/fcc-introduces-rules-banning-wifi-router-firmware-modification/>

多年来，我们一直受到廉价消费电子产品的青睐，这些产品可以通过非官方手段升级。你的任天堂 DS 能够运行未签名的代码，你的旧 XBox 在当时是一个有能力的服务器，你的 Android 智能手机可以通过 CyanogenMod 变得更好，由于开源固件创作者的努力，你的无线路由器可以扩展到远远超出最初设计的功能。现在，这种情况可能会改变。在美国联邦通信委员会提出的一项规则中，[带有无线电的设备可能需要防止固件修改](https://apps.fcc.gov/kdb/GetAttachment.html?id=1UiSJRK869RsyQddPi5hpw%3D%3D&desc=594280%20D02%20U-NII%20Device%20Security%20v01r02&tracking_number=39498)。

提议的规则只影响工作在 [U-NII 频段](https://en.wikipedia.org/wiki/U-NII)的设备；用于 5GHz WiFi 的那部分频谱，提议的规则只影响这些设备内部的*无线电*。像所有的政府法规一样，意外后果法抬起了它丑陋的头，拟议中的规则有效地禁止了开源路由器固件。

[规则要求所有相关设备](https://apps.fcc.gov/oetcf/kdb/forms/FTSSearchResultPage.cfm?id=39498&switch=P)实施软件安全，以确保在该频段运行的设备的无线电不被修改。由于廉价路由器的经济性，几乎每个路由器都是围绕片上系统设计的——在单个封装中集成 CPU 和无线电。禁止修改一个不可避免地会禁止修改另一个，并消除了在任何设备上安装经过验证的开源固件的可能性。