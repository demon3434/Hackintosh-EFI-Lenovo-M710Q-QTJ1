# Hackintosh-EFI-Lenovo-M910Q-QTJ1
## 联想M910Q，魔改QTJ1(i9 10980HK ES)，黑苹果EFI

首先感谢[原作者](https://github.com/Devinyu0616/Lenovo-M710Q-QTJ1-94360z4-Hackintosh)，我仅是做了较小的修改，以适配我的自选硬件。

### 软件版本
| 软件 | 版本 |
| --- | :--: |
| 系统 | macOS Monterey 12.3.1 (21E258) |
| 引导 | OpenCore v0.8.0 |

### 自选硬件
|   硬件    |   型号  |
| -------- | :----: |
| 主机 | 联想M910Q 魔改BIOS（青蛙家购买） |
| CPU | Intel Core i9 10980HK ES (QTJ1) |
| 内存 | 玖合 DDR4 2666 16GB*2 |
| 硬盘 | 西部数据 黑盘 SN750 1TB |
| 显卡 | AMD RX460 4GB(免驱)，屏蔽UHD630核显 |
| 显示器 | DIY便携屏，4K 60Hz |
| 无线网卡 | 白苹果拆机 BCM94360CS2 |

### 完成度
+ 独显免驱，屏蔽核显（不屏蔽核显，安装卡代码）
+ 声卡可以驱动
+ Wi-Fi、蓝牙正常驱动，由于是白苹果拆机网卡，隔空投送完美
+ 睡眠可唤醒
+ USB定制，USB接口正常（后方从上向下第3个USB接口，不识别USB2.0设备，不清楚是魔改BIOS问题，还是我的机器故障）
+ 魔改的另一个NVMe硬盘装Win10，OC可引导Win10
+ 引导界面图形化，开机有“duang”声音

### 缺陷
+ 不知道是网卡问题，还是驱动没配置好，蓝牙搜不到音响，能搜到手机，但双向隔空投送正常

### 备注
1. PlatformInform 模拟机型，DataHub的机型选择“iMac20,2”，Generic的机型选择“Macmini8,1”
2. 由于本人使用4K显示器，故设置了UIScale=02；如果用1080P显示器，苹果logo会显得巨大，请自行到nvram的“4D1EDE05-38C7-4A6A-9CC6-4BCCA8B38C14”中，修改UIScale为01
3. 如需使用此EFI，请***务必重新三码摇号***（适合OpenCore v0.8.0的OCC编辑器已放入本仓库，[图文教程](https://blog.csdn.net/xuanxue11/article/details/107873835)）

### 效果图
![关于本机.png](https://github.com/demon3434/Hackintosh-EFI-Lenovo-M910Q-QTJ1/blob/master/OpenCore%20v0.8.0%20%26%20macOS%2012.3.1%20(21E258)/%E5%85%B3%E4%BA%8E%E6%9C%AC%E6%9C%BA.png "关于本机")
![PlatformInfo机型选择.png](https://github.com/demon3434/Hackintosh-EFI-Lenovo-M910Q-QTJ1/blob/master/OpenCore%20v0.8.0%20%26%20macOS%2012.3.1%20(21E258)/PlatformInfo%E6%9C%BA%E5%9E%8B%E9%80%89%E6%8B%A9.png "PlatformInfo机型选择")
