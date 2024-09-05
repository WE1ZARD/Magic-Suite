## 1.4.2
- 修复cpu table auto针对高speedo优化
- 新增Shift Fix 1: 防止table切换
- 新增Shift Fix 1: 防止table切换, 明显降低中频电压

## 1.4.1
- kip增加8G时序
- CPU高频vmin改为710mv
- 新增CPU 2499档位锁定
- 改善CPU Table Auto兼容性
- gpu_volt_mariko.py更新改善后uv1表
- 更新sys-clk-oc EOS-1.0.1: 修复CPU2600+的实时频率bug

## 1.4.0b
- 更新Tesla-pro 3.1.6: 修复优先bug
- 更新Status Monitor 1.1.3a: 微调间距, 修复nx-fancontrol冲突
- 更新Updater 0.1.1: Update AIO 不再覆盖`settings.ini`, `hekate_ipl.ini`
- 设置add_defaults_to_dns_hosts=u8!0x0, 解除真实系统联网屏蔽

## 1.4.0a
- 更新Tesla-pro 3.1.5
- 新增USB 3.0补丁
- 修复大气层开机画面亮度问题, 现在和switch logo相同
- ultracam 降回2.1.4
- 更新R2Config 0.0.2, 内置进整合包
  - 优化显示逻辑
  - 新增`Reboot To > Hekate` 重启到Hekate引导界面
  - 新增`Set Launch`, 设置开机启动HOS还是Hekate菜单
## 1.4.0
- 修复status monitor > micro 字符串长度不够导致重叠显示
- 更新ultracam 2.5.0, benchmark启动快捷键`ZL+ZR+LS`
- 更新Settings 0.1.6
- 将`settings.ini`录制设置设为默认, 可以解决无法传输手机的问题
- mariko `GPU UV1` 优化
- GPU 1305mhz 只能UV2或者UV3才能使用
- CPU Low Freq Vmin 默认改为 `620mv`
- CPU 新增 `Table Config`, 调整High Freq分段
  - Auto: 根据Vmin和UV自动调整
  - Default: 默认无修改
  - 1581 Mhz: 高频从1581开始
- 新增时序 `tRTW`
- 去掉时序 `tWRWR` , `tRDRD`
- 主时序改回选项序号
- 默认tRFC新增`90` `50` `40`
- 移除 `AUTO_ADJ_LV`
- 调整magic > configure 排序
- magic加入更新覆盖kip确认
- 更新Tesla Pro 3.1.4, 增加新时序支持
- 更新MemToolkitNX 1.1.0, 支持读取超频参数
- 更新sys-clk-oc EOS-1.0.0, 支持读取超频参数
- 更新Status Monitor 1.1.2配置模板文件和默认设置
- 更新Settings 0.1.5, 增加Game模块

## 1.3.7
- 去掉status monitor的默认config.ini
- 更新FPSLocker 2.0.1-magic, 修复刷新率导致死机的bug
- 修复Updater错误序号导致无法正常更新, 0.1.0以下的版本需要手动覆盖更新updater
- 更新Updater 0.1.0
- tRFC4新增92-98
- 去除插件分隔线
- 更新Status Monitor 1.1.2
- 更新Settings 0.1.4
- CPU频率上限锁定, 新增1963Mhz
- 无UV下CPU的最大频率现在改为1963Mhz
- GPU U2电压微调
- 1075Mhz的GPU电压增加对高speedo的兼容

## 1.3.6
- vdd2电压调整为912.5-1350mv
- vddq电压调整为370-650mv

## 1.3.5
- 修复updater错误路径
- 移除hekate中强制开启usb3.0
- 新增时序预设 `Magic > Configure > TIMING > Presets`
- 更新Settings 0.1.3, 新增系统报错记录清理
- 更新tesla pro 3.0.2, 采用新的backup名称和版本编号
- 更新cpu最大电压范围为900-1235mv
- DVB现在允许降低电压选项 `-1, -2`, `soc speedo > 1633` 可用
- mariko CPU最大电压现在解锁到1235mv, 比较危险, 不建议用最高电压
- 更新Status Monitor 1.1.2
- 更新MemToolkitNX 1.1.0
- 更新SaltyNX 0.9.2, 兼容skyrim

## 1.3.4
- 新增Full模式和Mini模式分辨率显示
- 更新Status monitor 1.1.1
- 更新SaltyNX 0.9.1
- 更新Status monitor 1.1.0
- 更新SaltyNX 0.9.0
- 更新Settings 0.1.2
- 新增超频参数最后记录
- 调整erista部分参数范围
- 加入1672 speedo
- CPU UV和High UV拆分, UV0-8, HIGH UV0-12
- 更新JKSV-webDAV 2024.8.1
- 添加AMS缺失的MTC tables
- 移除ADJ_LV_HP
- 更新Updater 0.0.5
- 调整GPU UV2电压(1267mhz电压明显降低了)
- DVB可选范围增加
- tRAS最低可以选17

## 1.3.4-pre
- 更新Telsa Pro 3.0.1
- 更新Updadater 0.0.3
- 新增R2Config模块, 允许重启到Android, Lakka, L4T
- 更新Settings 0.1.0
- 增加时序序号, 新增NME, NEI颗粒预设
- 更新EdiZon, 改成打开直接显示金手指
- 更新Updater 0.0.2
- 更新JKSV 7.18.2024官方版
- 新增Updater更新模块, 支持HOS内一键更新
- settings.ini 开启金手指启动项保存
- Settings更新到0.0.9, 新增EdiZon金手指设置
- 更新全部解压密码```https://github.com/WE1ZARD```, 旧密码```https://afdian.net/a/weizard``` 只能用于1.3.4之前的版本
- 新增magic-suite展示页开源项目https://github.com/WE1ZARD/Magic-Suite
- 更新CPU帮助文件
- 新增CPU UV0-12
- 新增mhr.nro CPU频率实时监控工具

## 1.3.3
- 增加mhz.nro cpu频率测试工具
- 把HP mode开关显示从数字0 1 改成 OFF ON
- 增加TX芯片的引导支持
- 添加更多的tRAS值
- 修复导入配置的错误长度
- 新增HP mode选项, 默认关闭, 开启可以提高性能, 大幅降低延时, 但是会明显发热和耗电
- 新增Unlock CPU选项, 默认开启, 解锁2601频率
- 新增HP mode 高性能模式, 提高性能的同时会增大功耗和升温
- 移除AUTO_ADJ_HP

## 1.3.2
- 修复全新换包kip没有正常生成导致的报错
- 更新hekate 6.2.1 & nyx 1.6.3
- FPSLocker解锁屏幕刷新率75hz
- 更新Settings 0.0.8(新增USB 3.0开关, 后台服务开关)
- 调整刷新率数值, 调整FPSLocker UI
- 更新SaltyNX 0.8.0, 修复底座不能自动恢复屏幕刷新率, 可能导致的死机
- 更新FPSLocker 2.0.0(允许刷新率超频, 移除警告, 上限加到70)
- 更新Status Monitor 1.0.4(屏幕刷新率功能兼容修复)
- 金手指个数限制从128个增加到255个
- 进一步优化GPU体质差的最小电压
- 更新sys-clk-oc oc8-616(修复电压和睿频的bug)

## 1.3.1
- 修复importer.ps1 bug
- 修复exporter.ps1存在多个文件时的导出错误
- 微调GPU Speedo低的GPU vmin
- FPSLocker加入屏幕刷新率调整模块(仅限LCD屏幕)
- 更新SaltyNX 0.7.5
- 调整多个插件的UI

## 1.3.0
- 升级hekate 6.2.0 v4, 修复初代机无法启动到L4T系统
- 无痛升级现在会自动移除主题相关的文件避免开不了机
- 不再包含[ldnmitm LanPlay私服联机插件](https://www.jianguoyun.com/p/Df3tCWMQ88W1DBiuoMkFIAA), [MissionControl 第三方蓝牙手柄](https://www.jianguoyun.com/p/DXU7rlQQ88W1DBiSs70FIAA), [Sys-Con 第三方有线手柄](https://www.jianguoyun.com/p/De6_85EQ88W1DBixoMkFIAA) (自行下载)
- GPU自动最小电压微调
- 微调初代机CPU UV4
- 更新蓝牙手柄MissonControl 0.11.1
- 更新大气层1.7.1 hekate6.2.0 支持18.1系统(含sigpatches)

## 1.2.7
- 更新ovlEdiZon.ovl[更新日志](https://www.jianguoyun.com/p/DTkxcPwQl8W1DBiF8sgF)
- Lockpick_RCM更新至1.9.12, 支持18.0.0系统key
- 修改Tesla-Pro Slider样式
- 修复不能正确生成loader.kip的问题
- 修复./switch/prod.key不存在导致的报错问题
- 大气层更新到最新的atmosphere-1.7.0-dev-4afc4210c
- 修复开启GPUboost不能使用GPU 1305mhz
- 内存上限提至3200
- 新增无痛升级 [无痛升级教程](https://www.jianguoyun.com/p/DVkHswgQgcS1DBiSz80FIAA)
- 新增AUTO_ADJ_LV_HP时序, 低压更紧的时序
- 初代机CPU现在有UV1-5, UV5是原来的UV3
- 初代机GPU UV3电压表独立出来

## 1.2.6
- 移除Init KIPs模块
- 移除KIP版本验证
- 新增MagicSuite初始化脚本(不再需要手动从.bak复制默认kip并改名loader.kip)
- 微调Micro模式间距
- Kip版本号更新
- AUTO_ADJ_2400改名为AUTO_ADJ_LV, AUTO_ADJ_LV非初代机的性能得到提升, 是一个更宽松的时序

## 1.2.5
- 修复了exporter.ps1导出时, Presets.json可能出现两个中括号的问题
- 修复一些小bug
- 改变CPU UV7 (UV6 high8 + 1428 MHz分段)
- 新增“AUTO_ADJ_2400”时序表, 帮助体质比较差的机子超到2400
- 统一时序表命名
- SysClk-oc修复初代机的电压bug
- 将全局设置合并到General层级

## 1.2.4-beta
- 微调部分GPU UV电压以提高稳定性
- 更新hbmenu使用最新的libnx, 并提供 [NSP版本](https://www.jianguoyun.com/p/DQnniwAQgcS1DBj-v9EFIAA)
- 为了系统稳定性, 将默认线程从4线程改为3线程, 新增Threads模块, 可以进行线程切换
- 新增Init KIPs模块, 首次全新换包设置好之后可以直接用Magic调频, 无须手动从.bak复制kip

## 1.2.4
- Erista
  - 修复休眠模式下的CPU UV 1-3

## 1.2.3
- 优化结构, 更新帮助文档
- 默认KIP的T1,T2,T3时序现在改为默认实际数值18-18-42, 不再采用0-0-0
- Erista
  - 改善GPU UV2, 提高稳定性
- Mariko
  - 自动调整GPU最小电压
  - 优化部分speedo的计算

## 1.2.2
- 更新Sys-clk-oc 8f3
- 更新Sys-clk-oc 8f2
- 所有powershell脚本由 ```旧城(C.C.)大佬```负责开发, 非常感谢!!!
- WIZARD现在支持一键导入配置(现在已支持导入自定义时序)
- 现在可以使用exporter来导出KIP配置
- 现在可以使用importer把配置写入KIP
- 修复包浆机UV2部分电压问题 
- 新增包浆机GPU降压等级
  - UV1 = 在Medel GPU静态降压曲线基础上整体+30mV
  - UV2 = 动态高降压等级(目前可能不太稳定)
  - UV3 = 静态电压

## 1.2.1
- GPU Speedo由原SPEEDO合并到GPU
- GPU Volt Max范围现在是800-850mv
- 关闭GPU Boost才可以使用1305mhz
- Perference现在增加GPU Speedo显示, CPU UV和HIGH UV显示在一行
- DVB现在erista和mariko分开成两张表以支持最新的变动
- erista CPU UV2&3现在最高支持到2295mhz
- erista DVB现在支持0-4, 共4档
- 合并更新了所有帮助菜单
- 引入WIZARD模块, 可以一键导入超频配置
- 实验性: 跨版本导入配置(不支持有新参数变化的跨版本)
- 实验性: 通过"字符串"分享超频配置
- 已知问题: 暂不支持从KIP文件导出配置,只能手动写配置文件, tRFC自定义时序暂时不支持

## 1.2
- 新增Erista UV0-3支持
- 变更Erista CPU Vmin 最低电压: 750-850mv
- 变更Erista CPU Vmax 最大电压: 1200-1257mv
- 内置Sigpatches
- 新增CPU High UV0-8
- 提高系统启动速度
- 添加18.0.1 nifm补丁
- 更新Settings 0.0.3
- Settings添加GPU Boost模块
- 默认kip初始值重新调整以兼容更多机器
- 修复mini模式下偶尔会出现部分读数空白的问题

## 1.1.1
- 提高CPU UV5-6的兼容性(部分机型原来无法开机的应该可以正常开机了)
- 旧UV8现改为UV7
- UV8 现在可以设置一个更低的高频最低电压
- Tesla-Pro 更新2.0.7
- Status Monitor监控FPW能效开关
- Status Monitor监控Volts电压开关
- FanControl风扇 & KeyCombo快捷键模块, 合并到Settings二级菜单
- 新增Record系统录制功能配置
- 帮助文件逻辑优化和订正部分错误的文本说明
- 修复部分Status Monitor的逻辑问题, 新增Settings对齐设置
- 更新status monitor 1.0.3c
- 更新Settings 0.0.2

## 1.1
  - 解锁CPU 2601
  - 增加CPU UV5-8
  - 解锁GPU 1305
  - Sysclk-oc 支持自动同步底座模式配置
  - 增加disable_remap_dialog
  - 更新SaltyNX 0.7.3
  - 移除comm

## 1.1-beta
  - tRCD, tRP, tRAS现在直接显示成实际值, 而不是选项值
  - 要求AMS 17.0 支持HOS 18.0.0
  - 采用扩展时序名
  - 增加sigpatches对18.0.0的支持
  - 支持EOS 1.1
  - MissonControl 蓝牙手柄插件支持18.0.0
  - Hekate增加recover恢复模式

## 1.0-beta
  - 主时序1拆分成3个独立的选项, 极限值进一步提高
  - WL-RL拆分成2个独立的选项, 以兼容更多颗粒
  - 支持EOS 1.0

## 0.5-beta
  - 增加CPU UV4
  - erista 初代机引入GPU UV1 自定义电压

## 0.4-beta
  - 提供4线程hbl
  - vdd2上限同步到1212mv
  - GPU Speedo +1626
  - 更新Y帮助菜单内容
  - EOS 0.4 支持
  - 修复自动存档kip命名规则

## 0.3-beta
  - 修复Telsa呼出bug
  - 修复ini文件不能正确生成的问题
  - Status Monitor引入实时电压
  - 超频管理插件更换为sys-clk-oc
  - 加入HekateToolBox
  - 使用eos 0.3 kip及Magic调频模块
  - 简化风扇控制UI显示
  - 更新hbl支持libnx 4.6.0
  - JKSV新增webDAV支持 [演示视频](https://www.bilibili.com/video/BV19J4m1a71j "跳转到Bilibili")
  - 重构了底层, 修复大量bug
  - 整合多个json列表, 优化packages载入速度
  - 修复部分cust转化不完全导致的bug
  - Tesla Pro修复小bug
  - 加入t2_tRRD-tFAW自定义时序(kip读取无法获取到时序的值, 所以暂不放进去)
  - 加入快捷键模块, 风扇控制模块
  - 超频设置里的所有值现在都可以正常显示出来, 包括自定义时序值
  - Preferences里添加自定义时序显示

## 0.2-beta
  - 优化了Tesla Pro的配置逻辑
  - 加入了kip版本号的验证
  - 加入了3组kip预设配置

## 0.1-beta
  - 已更新CPU UV配置文件
  - sigpatch文件重新覆盖最新的
  - 修复自定义tRAS和tRFC偏移量的错误
  - Y帮助文件已更新对应版本


```
 _____ ___ ___ _ __
|     |   |   | |  |  A Minimalistic CFW Of Overclocking.
| | | | - | |-| | -|
|_|_|_|_|_|___|_|__|  https://github.com/we1zard/magic-suite
```