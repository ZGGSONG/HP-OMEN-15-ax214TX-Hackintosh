# HP-OMEN-15-ax214TX-Hackintosh

[![img](https://img.shields.io/github/last-commit/ZGGsong/HP-OMEN-15-ax214TX-Hackintosh.svg?color=orange&label=%E6%9C%80%E8%BF%91%E6%8F%90%E4%BA%A4)](https://github.com/ZGGsong/HP-OMEN-15-ax214TX-Hackintosh) [![img](https://img.shields.io/badge/link-996.icu-red.svg)](https://996.icu/) 
[![GitHub release (latest by date)](https://img.shields.io/github/v/release/zggsong/HP-OMEN-15-ax214TX-Hackintosh)](https://github.com/ZGGSONG/HP-OMEN-15-ax214TX-Hackintosh/releases/)

## 注意

**更新为OC引导，使用的同学一定记得改三码，apple id被封了概不负责（务必关闭查找）**

## 配置
| 分类 | 说明 |
|:----:|:----:|
| 型号 | HP暗影精灵 II 代Pro |
| CPU | i5 7300HQ |
| 网卡 | DW1560/BCM94352Z |
| 集显 | HD630 |
| 独显 | GTX1050 |
| 声卡 | ALC295 |

<details>
  <summary>   </summary>

## 2.2 更新

- 支持macos11.2.3
- 请于[release](https://github.com/ZGGSONG/HP-OMEN-15-ax214TX-Hackintosh/releases)页面下载最新版本

## 2.1.1更新

- 添加`DW1560`网卡驱动

- 修改序列号(每个人自己用记得修改)

如有需要[点击下载](https://zggsong.lanzous.com/imxmtipssqf)

```
DW1560黑苹果驱动，适用于macOS Catalina 10.15.1、macOS Catalina 10.15.2、macOS Catalina 10.15.3系统。

如果你的机型需要屏蔽针脚，请先屏蔽好针脚才能驱动Wi-Fi。

安装方法：

CLOVER引导

安装到CLOVER\Kexts\Other 目录下，重启即可。如果没有效果重启进mac之后重建缓存之后再重启即可。

OpenCore引导

安装到OC\Kexts 目录下，Config.plist添加好驱动然后重启即可。如果没有效果重启进mac之后重建缓存之后再重启即可。
```

- 转自[http://www.macoshome.com/hackintosh/hdrivers/2486.html](http://www.macoshome.com/hackintosh/hdrivers/2486.html)

> **此处EFI分为两个版本：（10.13.6 && 10.14.4）和 10.15.3 两个版本**
> > 此处我指明具体系统版本是我本人体验过的版本，目前10.15.3运行十分良好

## 下载

[**点击下载**](https://github.com/ZGGSONG/HP-OMEN-15-ax214TX-Hackintosh/releases)

> 版本自行选择

## 总结

经历两次大规模折腾，现今EFI已经解决：

**电源电量、声卡、蓝牙、键盘快捷键、CPU睿频、HIDPI（手动开启，下面历程有介绍）**

***注意：睡眠（指的是电脑进入睡眠，并不是指显示器）后发热量巨大，（本人并非大佬）查找很多资料无果，在此提醒***

无解：**wifi（需购置）、独显无解（HDMI接口独显输出，如果连接显示器也可以USB转HDMI）**

<details>
  <summary>如果很迷恋多指手势，请看这里（触控板使用效果并不好，常常识别错误，就没加在里面）</summary>

> 触控板手势仅有单指和双指，更多手势可下载此处根目录的[ApplePS2SmartTouchPad.kext.zip](https://github.com/ZGGSONG/HP-OMEN-15-ax214TX-Hackintosh/raw/master/ApplePS2SmartTouchPad.kext.zip)，解压后替换`/EFI/Clover/kexts/other/VoodooPS2Controller_v1.9.2.kext`驱动即可获得三指等手势，但亮度快捷键会无效且`option`和`command`位置会互换，当然，可以通过修改`info.plist`来修改（之前改了一个比较完美的，忘记留了，不过各位意义真不大，你可以换这个试试😂）
</details>

**⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️（*可忽略*）**


## 历程
---
10.13.6 && 10.14.4
---
## ☛ 倒腾黑苹果

倒腾黑苹果几个星期，终于有所收获，大体配置好了一份自己电脑可以用的EFI文件，现分享出来，供同款电脑拥有者使用~

## 解决问题

 - 睡眠后完美启动

 - 电源补丁打好，不会一直显示100%(如果电量不掉那就是静电问题，关机长按20s电源即可)

 - 声音完美解决(别作死热启动，别问为什么，都是泪)

## 存在问题
 - HDMI接口无法使用（独显驱动）

 - 你知道的——WIFI，无解，某宝了解一下([黑苹果usb网卡CF-811AC驱动美化and汉化](https://zhebk.cn/Z-Turn/CF-811AC.html))

 - 触控板手势无法使用，尝试过很多方法，失败告终(有解决了的，可以分享一波)

 - 在使用10.14.4的时候，温度挺高的，在10.13.6也没那么高，不知道是不是错觉(CPU睿频了，独显屏蔽了)，如果你们没有的话，就应该是我电脑该换硅脂了。。。

---
10.15.3
---

## 升级

mac OS 10.13.6升级到mac OS 10.15.3

> 个人感受比较明显的就是速度的提升，从开机到整体的运行都更加的流畅了（咳咳，忘了身份【黑苹果玩家偷笑ing】）

## 分享

本人电脑中的软件基本都有：

[**点击下载**](https://zggsong.lanzous.com/b0ck8dtgj
) **密码:6812**

> 其中尤其推荐**Smooze**这个软件（鼠标手势app）

## 注意

- 电脑开启HiDPI [**https://www.sqlsec.com/2018/09/hidpi.html**](https://www.sqlsec.com/2018/09/hidpi.html)

- HP暗影精灵2pro经实测无法开启独立显卡，由于HDMI口是独显输出，所以HDMI没办法用（并且要做好独显屏蔽工作，否则发热量巨大）

- <b style="color:red">实测win下屏蔽独显外接显示器显示，但是Hacnintosh可通过隔空投送到网络显示器：电视（无需更换网卡也可以实现）</b>

- WIFI需要另外购置，几款特殊型号可支持AirDrop，随航等功能

## 截图

> 图国内途径 [**https://blog.zggsong.cn/archives/1065.html**](https://blog.zggsong.cn/archives/1065.html)
![](https://cdn.zggsong.cn/2020/03/21/142060289abd1.png)

![](https://cdn.zggsong.cn/2020/03/21/0249761a4bfa9.png)

![](https://cdn.zggsong.cn/2020/03/21/b26e0df46f6ee.png)

![](https://cdn.zggsong.cn/2020/03/21/a7cfea9c177a8.png)

![](https://cdn.zggsong.cn/2020/03/21/949814e3c55e8.png)

![](https://cdn.zggsong.cn/2020/03/21/b3c327f858af2.png)

![](https://cdn.zggsong.cn/2020/03/21/f393788e1fcf1.png)

![](https://cdn.zggsong.cn/2020/03/21/43d85ea996bbd.png)

![](https://cdn.zggsong.cn/2020/03/21/99273658b4f01.png)

 ## 其他问题，请移步

<div>
 <b><a href="https://blog.daliansky.net/" target="_blank">黑锅小兵</a>
 </div>
 <div>
 </b>
 <b><a href="http://bbs.pcbeta.com/index.php?gid=86" target="_blank">远景论坛</a></b>
</div>
</details>
