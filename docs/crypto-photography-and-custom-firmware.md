# 加密摄影和定制固件

> 原文：<https://hackaday.com/2014/12/18/crypto-photography-and-custom-firmware/>

想象一台拍摄加密照片的相机。如果你的相机被偷了，存储卡上唯一的东西就是随机数据，只能用钥匙解锁。如果你雇了一个摄影师，没有钥匙这些图像是无法复制的。至少，这是一个有趣的想法[令人印象深刻，因为它确实存在](https://sites.google.com/site/nxcryptophotography/home)。

[Doug]最近得到了一台三星 NX300，这是一台不错的相机，价格适中，可以方便地运行 Linux，并且是三星的开源产品。通过特殊的固件，[Doug]为这台相机创建了公钥/私钥加密，只有拥有私钥的人才能解锁这台相机拍摄的照片。

[Doug]通过查看这个相机的固件开始他的构建，想出如何将所有东西拆开并重新组装起来。经过一些修改(包括对这台相机拍摄的所有图像进行加密)，[Doug]重新打包了固件并升级了相机。

加密固件[可以在网站](https://sites.google.com/site/nxcryptophotography/downloads)上获得，但是考虑到【Doug】能够如此容易地使这种攻击发生，以及如何实际做到这一点的一个很好的演练提出了一些有趣的可能性。NX300 是一款相当不错的相机，比由 [CHDK](http://chdk.wikia.com/wiki/CHDK) 支持的佳能 PowerShot 相机略高一点。它也运行 Linux，所以如果你想用一个漂亮的相机做一些很酷的事情，[道格]有一个非常好的资源。