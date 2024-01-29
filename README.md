# Asus-TUF-Z390-9900K-6600XT-EFI
- 支持系统：Monterey 12.x、Ventura 13.x、Sonoma 14.x 
- 请自行生成修改Board Serial Number、序列号、SmUUID等三码信息
- EFI(独显/集显可选) [点击下载](https://github.com/lwf1127/Asus-TUF-Z390-9900K-6600XT-EFI/releases)
  
![输入图片说明](image/macos.png)
#### 20240129更新：
1. 独显6600XT，升级到MacOS14.3,OC0.9.7正式版。博通网卡需要搭配OCLP补丁使用。 https://github.com/dortania/OpenCore-Legacy-Patcher
2. 集显HD630在MacOS14下，已无法流程运行，交互动画会丢帧卡顿，后续将不再更新。

#### 20231016更新：
1. 独显6600XT，升级到MacOS14。支持4k144hz可变刷新率,支持HDR,原生支持HiDPI。从此，黑果再无短板！
   
#### 20231007更新：
1. 集显HD630，升级到 MacOS14。OCLP1.0.1完美支持博通网卡。隔空、通用、互通一切正常。
  
#### 20230925更新：

1. 独显6600xt长期稳定版,oc-0.9.4-开发版,MacOS13.4
2. 集显HD630,oc-0.9.6-开发版,MacOS13.6
3. 定制USB端口,解锁15个USB口上限
   
#### 20230220更新：

1. 解决在Windows下主板名称不正确的问题。参考：https://www.bilibili.com/read/cv9278654

#### 20230210更新：

1. 如在开机时发现主板自检阶段时间过长，显示器很久才能点亮，请在Kernel-》Quirks-》勾选：DisableRtcChecksum(禁用RTC校验)


#### 硬件配置：
- CPU ：i9-9900K
- 主板 ：华硕(ASUS)TUF Z390-PLUS GAMING (WI-FI) 电竞特工主板
- 内存 ：DDR4 3200 8G*2 16G
- 显卡 ：技嘉RX6600XT 魔鹰PRO
- 硬盘 ：海康威视 C2000Pro 500G
- 板载网卡：Intel有线网卡+Intel® Wireless-AC 9560
- 板载声卡：Realtek® S1200A
- 无线网卡：BCM943602CDP(白果拆机卡)+PCIE转接卡
- 散热：利民 Magic EX 240水冷

#### BIOS设置：

- 【高级】 - 【CPU 设置】 - 【软件保护扩展（SGX）】- 【关闭】
- 【高级】 - 【CPU 设置】 - 【Intel VMX 虚拟化技术】 - 【开启】
- 【高级】 - 【CPU 设置】 - 【CPU-Power Management Control】 - 【CFG Lock】 - 【关闭】
- 【高级】 - 【北桥设置】 - 【大于4G地址空间解码】 - 【开启】
- 【高级】 - 【北桥设置】 - 【显示设置】 - 【首选显卡】 - 【auto】
- 【高级】 - 【北桥设置】 - 【显示设置】 - 【初始化iGPU】 - 【开启】
- 【高级】 - 【北桥设置】 - 【显示设置】 - 【DVMT Pre-Allocated】 - 【最大】
- 【高级】 - 【PCH存储设置】 - 【SATA摸式选择】 - 【AHCI】
- 【高级】 - 【USB Configuration】 - 【XHCI Hand-off】 - 【开启】
- 【启动】 - 【启动设置】- 【快速启动】 - 【关闭】
- 【启动】 - 【若出现错误等待按下F1键】  - 【关闭】
- 【启动】 - 【CSM(兼容性支特摸块)】 - 【开启CSM】 - 【关闭】
- 【启动】 - 【安全启动菜单】 - 【操作系统类型】 - 【其他操作系统】

#### 完善程度：
1. CPU 跑分正常，H264、HEVC硬解正常
2. USB 2.0 和3.0正常
3. 有线网卡、WIFI、蓝牙正常
4. 支持隔空、通用控制、手机相机连续互通
5. 音频输出正常
6. 睡眠与唤醒正常
7. TRIM支持正常
8. USB额外操作电流、睡眠电流正常
9. 显卡Metal支持正常
10. CPU、显卡、风扇温度转速显示正常

#### 部分截图：
![输入图片说明](image/amd-gpu.png)
![输入图片说明](image/wifi.png)
![输入图片说明](image/ble.png)
![输入图片说明](image/dpi.png)

#### OpenCore & Kext：
![输入图片说明](image/acpi.png)
![输入图片说明](image/dp.png)
![输入图片说明](image/kernel-3.png)
![输入图片说明](image/boot-args.png)


#### USB定制：
![输入图片说明](image/usb-2.png)

#### 鸣谢：
- EFI参考：https://github.com/jhihhe/Hackintosh-Asus_Prime_Z390P-i9-9900K_UHD630-RX-6600XT-EFI_OpenCore-0.8.8-macOS
- 国光的黑苹果安装教程：https://apple.sqlsec.com/
- IT记：https://hackintosh.myitnote.com/
- OSX：https://osx.cx/
- 远景论坛：https://bbs.pcbeta.com/forum.php?gid=86
- 黑苹果星球：https://heipg.cn/
- 黑果小兵：https://blog.daliansky.net/Hackintosh-long-term-maintenance-model-checklist.html#asus-%E5%8D%8E%E7%A1%95-1
