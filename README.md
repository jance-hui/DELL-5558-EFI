# DELL-5558-EFI
**戴尔灵越15-5558型号电脑黑苹果EFI**

电脑配置（硬件信息来自鲁大师）：

规格     | 详细信息
-------- | -----
电脑型号  | 戴尔 Inspiron 15-5558 笔记本电脑
操作系统  | macOS Mojave 10.14.4(18E226)
处理器  | 英特尔 Core i5-5200U @ 2.20GHz 双核
主板  | 戴尔 0WMF3P ( 5th Generation Intel Core Premium SKU - 9CC3 笔记本芯片组 )
内存  | 8 GB ( 镁光 DDR3L 1600MHz )
主硬盘  | 西数 WDC WD5000LPVX-75V0TT0 ( 500 GB / 5400 转/分 )
核显  | Intel Graphics HD 5500
集显  | Nvidia GeForce 920M ( 2 GB ) **（集显不可用）**
显示器  | LG LGD0484 ( 15.5 英寸  )
光驱  | PLDS DVD+-RW DU-8A5LH DVD刻录机
声卡  | 瑞昱  @ 英特尔 High Definition Audio Controller
网卡  | 英特尔 Dual Band Wireless AC 3160 **（注意：无线网卡需自行更换Atheros AR9565）**

安装镜像：[黑果小兵10.14.4（18E226）](https://blog.daliansky.net/macOS-Mojave-10.14.4-18E226-official-version-with-Clover-4903-original-image.html
)， clover已自行升级为4915

clover主题已根据给本人喜好更换，也可在`CLOVER/config.plist`搜索`theme`更换自己喜欢的主题（注：主题需放在`CLOVER/themes`下）


**安装时请使用镜像自带Clover，安装完成后替换此EFI**

正常功能：

- 1、核显驱动正常，用的镜像EFI里config_5300_5500_6000.plist
- 2、USB2.0，3.0正常，facetime摄像正常
- 3、声卡使用万能驱动，外放正常，麦克风正常，耳机需把平衡拉到最左或最右不然有杂音
- 4、睡眠唤醒正常。亮度调节删除COLVER里有关亮度驱动，config里ACPI添加PNLF,有小太阳
- 5、HDMI可以输出，我用的HDMI转VGA
- 6、有线无线正常，DW1707速度够用,clover里面有WiFi和蓝牙驱动，但是蓝牙用不了

EFI驱动等文件均来自于远景论坛大佬制作，本人小改了一下主题

远景大佬帖子：http://bbs.pcbeta.com/viewthread-1811188-1-1.html