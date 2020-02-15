# HP-OMEN-15-ax214TX-Hackintosh

[![img](https://img.shields.io/github/last-commit/ZGGsong/HP-OMEN-15-ax214TX-Hackintosh.svg?color=orange&label=%E6%9C%80%E8%BF%91%E6%8F%90%E4%BA%A4)](https://github.com/ZGGsong/HP-OMEN-15-ax214TX-Hackintosh) [![img](https://img.shields.io/badge/link-996.icu-red.svg)](https://996.icu/) 
[![GitHub release (latest by date)](https://img.shields.io/github/v/release/zggsong/HP-OMEN-15-ax214TX-Hackintosh)](https://github.com/ZGGSONG/HP-OMEN-15-ax214TX-Hackintosh/releases/tag/1.0.0)


## 配置
| 分类 | 说明 |
|:----:|:----:|
| 型号 | HP暗影精灵 II 代Pro |
| CPU | i5 7300HQ |
| 集显 | HD630 |
| 独显 | GTX1050 |
| 声卡 | ALC295 |



> **此处EFI分为两个版本：（10.13.6 && 10.14.4）和 10.15.3 两个版本**
> > 此处我指明具体系统版本是我本人体验过的版本，目前10.15.3运行十分良好

## 下载

[**点击下载**](https://github.com/ZGGSONG/HP-OMEN-15-ax214TX-Hackintosh/releases/tag/2.0)

> 版本自行选择

## 总结

经历两次大规模折腾，现今EFI已经解决：**电源电量、声卡、蓝牙、键盘快捷键、CPU睿频、HIDPI（手动开启，下面历程有介绍）**

无解：**wifi（需购置）、独显无解（HDMI借口独显输出，如果连接显示器也可以USB转HDMI）**

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

> [https://pan.baidu.com/s/1C-Bs61SLPksHbqAgHUUS1w](https://pan.baidu.com/s/1C-Bs61SLPksHbqAgHUUS1w) 

> 提取码: j1s7

> > 其中尤其推荐**Smooze**这个软件（鼠标手势app）

## 注意

- 电脑开启HiDPI [**https://www.sqlsec.com/2018/09/hidpi.html**](https://www.sqlsec.com/2018/09/hidpi.html)

- HP暗影精灵2pro经实测无法开启独立显卡，由于HDMI口是独显输出，所以HDMI没办法用（并且要做好独显屏蔽工作，否则发热量巨大）

- WIFI需要另外购置，几款特殊型号可支持AirDrop，随航等功能

## 截图

> 图国内途径 [**https://blog.zggsong.cn/archives/1065.html**](https://blog.zggsong.cn/archives/1065.html)
![截屏2020-02-14上午3.34.53.png](https://img.zggsong.cn/2020/02/14/f2bade2641d5d.png)

![截屏2020-02-14上午3.35.30.png](https://img.zggsong.cn/2020/02/14/2507dee93dcd4.png)

![截屏2020-02-14上午3.35.35.png](https://img.zggsong.cn/2020/02/14/988f5df40db20.png)

![截屏2020-02-14上午3.35.42.png](https://img.zggsong.cn/2020/02/14/a16feeb828bbf.png)

![截屏2020-02-14上午3.35.46.png](https://img.zggsong.cn/2020/02/14/4db57b67cbeee.png)

![截屏2020-02-14上午3.36.22.png](https://img.zggsong.cn/2020/02/14/cfc2460b2b1be.png)

![截屏2020-02-14上午3.37.11.png](https://img.zggsong.cn/2020/02/14/a5ccddf8eae5c.png)

![截屏2020-02-14上午3.37.19.png](https://img.zggsong.cn/2020/02/14/269576c68a1ae.png)

![截屏2020-02-14上午3.37.28.png](https://img.zggsong.cn/2020/02/14/8d11300b96ff7.png)

![截屏2020-02-14上午3.37.55.png](https://img.zggsong.cn/2020/02/14/1162286d40224.png)

![截屏2020-02-14上午3.38.00.png](https://img.zggsong.cn/2020/02/14/b757b7bc682ef.png)

 ## 其他问题，请移步

<div>
 <b><a href="https://blog.daliansky.net/" target="_blank">黑锅小兵</a>
 </div>
 <div>
 </b>
 <b><a href="http://bbs.pcbeta.com/index.php?gid=86" target="_blank">远景论坛</a></b>
</div>
