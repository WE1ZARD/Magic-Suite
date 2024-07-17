<p align="left">
<a href="https://creativecommons.org/licenses/by-nd/4.0/deed.zh-hans"><img alt="CC BY-ND 4.0-CN)" src="https://img.shields.io/badge/License-CC%20BY--ND%204.0-lightgrey.svg"></a>
<a href="https://github.com/WE1ZARD/Magic-Suite/releases/latest"><img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/WE1ZARD/Magic-Suite"></a>
<a href="https://github.com/WE1ZARD/Magic-Suite/releases"><img alt="GitHub All Releases" src="https://img.shields.io/github/downloads/WE1ZARD/Magic-Suite/total"></a>
<br>
</p>

# Magic Suite
此项目仅为展示SWITCH硬件潜能学习交流之用, 非以盈利为商业目的.

## 使用须知
- 超频可能导致(包括但不限于): 引起系统不稳定, 破坏, 发热, 耗电, 损坏硬件等可能的后果
- 建议只在虚拟系统使用, 并且折腾前做好完整的备份, 以免造成不可挽回的损失.
- 使用者自行承担可能的存在风险和后果, 本人概不负责.

## 基本操作
- **L + 加号** 呼出特斯拉菜单
- **左摇杆 + 右摇杆** 退出监控插件
- 更多操作说明: 见压缩包user_guide.md

## 交流和支持
- [QQ群](https://qm.qq.com/q/RYsABoQpi0): ```737375560```
- [DC群](https://discord.gg/kZDgtSPQCn): ```Magic-Suite```
- [爱发电](https://afdian.com/a/weizard): ```weizard```

## 全新安装说明

- 先自己备份好文件之后, 保留以下文件
```bootloader/ini/``` ```emuMMC``` ```JKSV``` ```lakka``` ```Nintendo``` ```switchroot```
- 之后将解压出来的```Magic-Suite```里的文件全部复制到根目录, 重启即可.(需要在Hekate > USB模式, 或者拔卡操作, **不能用MTP操作**)

## 无痛升级说明
**请尽量避免从别的整合包使用直接升级教程的方法, 可能会出现兼容方面的问题, 后果自负**
* 希望**保存自己Hakate引导配置**的朋友, 
提前将以下路径文件进行改名,
	- 原来: sd:/bootloader/```hekate_ipl```.ini
	- 改后: sd:/bootloader/```hekate_ipl_```.ini
```
├ bootloader
└ Magic-Suite
```
* 之后通过 **MTP**, **WIFI** 等方式把解压之后的这两个文件夹复制到```sd:/```, 并且**选择覆盖文件**.
不严格要求UMS模式或者拔卡操作.
* 复制完成之后, 正常重启Switch会进入自动更新程序, 更新完成之后会自动重启
默认重启到HOS, 保留自己配置的, 按照自己配置的引导
* 升级会保留**所有原先的系统配置**, 包括**金手指**/**MOD**, **各种补丁**(系统主题相关会被删除)

## 支持硬件
- SWITCH 初代
- SWITCH 续航版
- SWITCH OLED
- SWITCH LITE

## 特斯拉套件
- Magic-Suite
- Settings

## 可选插件
- [坚果云搬运地址](https://www.jianguoyun.com/p/DQ6eZFkQgcS1DBir4NgFIAA)

## 超频教程
- [SWITCH完整超频教程](https://www.bilibili.com/opus/953913305942982710)


<details>
<summary>包含哪些</summary>

- [Atmosphere](https://github.com/Atmosphere-NX/Atmosphere) (分支)
- [Hekate](https://github.com/CTCaer/hekate)
- [Hekate-Toolbox](https://github.com/WerWolv/Hekate-Toolbox)
- [Sigpatches](https://sigmapatches.coomer.party)
- [FPSLocker](https://github.com/masagrator/FPSLocker) (分支)
- [ReverseNX-RT](https://github.com/masagrator/ReverseNX-RT)
- [SaltyNX](https://github.com/masagrator/SaltyNX) (分支)
- [Uberhand-Overlay](https://github.com/efosamark/Uberhand-Overlay) (分支)
- [Status Monitor](https://github.com/hanai3Bi/Status-Monitor-Overlay) (分支)
- [DBI](https://github.com/rashevskyv/dbi)
- [Lockpick RCM](https://github.com/s1204IT/Lockpick_RCM)
- [TegraExplorer](https://github.com/suchmememanyskill/TegraExplorer) (分支)
- [JKSV](https://github.com/J-D-K/JKSV) (分支)
- [Linkalho](https://github.com/HamletDuFromage/linkalho)

</details>

<details>
<summary>特别感谢</summary>

- b0rd2dEAth
- b3711
- C.C.
- ChanseyIsTheBest
- CtC
- Efosamark
- lineon
- MasaGratoR
- meha
- DC社区: NSwitch 60FPS Cheats & Mods

</details>