---
layout: post
title: 将小米MIX 2刷成Android P初体验
author: 老马同学
tags:
- Xiaomi
- MIX 2
- Android P
- Flash
- ROM
- TWRP
- XDA
categories: Tutorial
english: false
---

我正在使用MIUI 10 EU的ROM，应该是``8.6.2``，是最稳定和省电的版本，一般使用一天到睡前还有20%的电（后面我会放出文件和刷机步骤）！

不过今天的主题是原生Android P。

这几天因为要查一个生产问题，所以终于决定将我的小米MIX 2刷成最新的Android Pie（Android 9）耍一耍，之前也一直有刷成原生系统的念头，不过知乎了一下，有很多玩家体验后，不是因为系统兼容性不好，就是因为掉电太快而最终放弃了。而我本身是有任务在身，所以好歹都要体验一把！不过这个ROM还很不完善，原本想写篇刷机步骤，但现在我已经打算刷回MIUI了。

## 刷机链接

如果你想折腾，这里把XDA的刷机办法放在这里给你参考。

[https://forum.xda-developers.com/mi-mix-2/how-to/how-to-flash-android-p-mi-mix-2-t3819334](https://forum.xda-developers.com/mi-mix-2/how-to/how-to-flash-android-p-mi-mix-2-t3819334)

在刷机之前，一定要做好备份。建议执行以下备份操作：

1. 如果你之前已经root了，推荐使用钛备份，可完美备份所有程序和数据。备份后会保存在``\sdcard\TitaniumBackup``下面，备份完成后将这个文件夹拷贝到你的电脑里。如果没有Root的话，最好先Root。非Root机器我还没有试过其他办法，可能保留不住你自己下载的APP和数据。
2. 备份MIUI的系统设置，以便将来刷回MIUI之用。备份后你可以到``\sdcard\MIUI\Backup\AllBackup``下面找到一个日期文件夹，将该文件夹拷贝到你的电脑里。

## 目前发现的问题

这个ROM还存在好多问题，这里面总结如下：

1. 偶尔会莫名其妙重启...（这点无法忍受）
2. 呼吸灯很亮...尤其是充电的时候，不过好消息是至少呼吸灯能用。所以晚上充电的时候就扣着充吧！
3. 外放声音有点问题，音质不是非常好，玩游戏（至少我玩皇室战争）声音有点破音。可装``Kernel Adiutor``，把``声音``的``耳机增益``调至``-10``。
4. 人脸解锁功能并不是很灵敏，远不如MIUI EU的版本。建议不要使用。
5. 没有自带的相机，需要额外安装。[点击此处下载 Google Pixel 2 相机](https://www.celsoazevedo.com/files/android/google-camera/f/GoogleCamera-Pixel2Mod-Arnova8G2-V8.apk)
6. 熄屏双击亮屏功能不起作用，可装``Kernel Adiutor``，把``双击唤醒``打开。指纹手势不起作用。目前无解。
7. 没有MIUI的安全中心，应用锁，骚扰拦截等功能，应用锁可安装``IVYMOBILE``的``应用锁``，骚扰拦截你可以用``Vlad Lee``的``电话拦截``。
8. Google服务在中国大陆无法使用，需要VPN。（这是原生系统的通病）
9. 震动的长度最短也是50ms左右，再往低设置也不起作用，也就是说不能轻微震动，例如使用Gboard打字的时候。可装``Kernel Adiutor``，把``杂项``的``震动强度``设置成``25%``。
10. 没有MIUI的全面屏手势，Pie带的手势功能很low。这里推荐一个韩国的App``Gesture Bar``，可以定义上下左右边框的各种手势操作，完全满足要求，但免费版只能定义底边手势。另外你也可以用``XDA Guesture``，但并没有左右侧边的手势定义。
11. NFC不起作用，使用不了公交卡。
12. 快充感觉比MIUI要慢。
13. 耗电在安装了``绿色守护``和``冰箱``以后，还是会掉的比MIUI快一点，而且电池计数器有问题，可能已经没电了，还显示有7%。没电了呼吸灯会狂闪。
14. 老是收到语音信箱的提示，又屏蔽不掉。在MIUI 10是可以屏蔽的。

## 新系统的优点

也有一些令人欣喜的地方：

1. 此ROM的兼容性非常好，各种硬件、传感器工作基本正常。
2. 原生系统高达上！配合动态桌面令人耳目一新。
3. 使用起来非常流畅。
4. 没有广告，没有注入的第三方服务。
5. 可以用``Ok Google``唤出Google助理。
6. 新的通知栏很酷，可以最小化通知，很赞！
7. Google的AI技术非常成熟，可以智能推送你喜欢的新闻，路况信息，航班信息等。
8. 集成了Google全家桶，Google应用和系统融合度高。