

# JLink_ARM_OB (STM32F072C8)
![](https://img.shields.io/badge/Version-1.2-brightgreen.svg)    ![](https://img.shields.io/badge/license-CC4.0-brightgreen.svg)
* Author: [DataSheep](https://github.com/JassyL/DAP_Link)
* Version: 1.2
* Update: 2017.12.06

# Description
JLink-OB (STM32F072C8)是基于STM32F072C8T6的一款JLink_OB下载仿真器，具有J-Link、ST-Link等相同功能，**并且支持虚拟串口**，方便调试。本版本基于[X893/CMSIS-DAP](https://github.com/x893/CMSIS-DAP)修改。
板载5V和3.3V输出，适合各种Cotex-M内核单片机。

不想自己做板子，可以上淘宝店:[数据羊电子](https://shop121585820.taobao.com)，出售空板和成品，价格将尽可能接近成本。

此版本JLink_ARM_OB增加了虚拟串口功能，并且使用STM32F072C8内部震荡，省去了外部晶振，PCB面积更小。

# License
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/deed.zh"><img alt="知识共享许可协议" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />本作品由[DataSheep](https://github.com/JassyL/DAP_Link)制作，采用<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/deed.zh">知识共享署名-相同方式共享 4.0 国际许可协议</a>进行许可。

# Photos
#### PCB
![JLink_ARM_OB](https://raw.githubusercontent.com/JassyL/github_photos/master/Jlink-OB-1_2.png)

#### 测试中照片
![JLink_ARM_OB](https://raw.githubusercontent.com/JassyL/github_photos/master/JLINK.jpg "1.2版实物")

![JLink_ARM_OB](https://raw.githubusercontent.com/JassyL/github_photos/master/tset_1.png "测试照片")

# Instructions for use
此版本没有留SW下载接口，可通过串口下载，下载前将背面BOOT0接高(详见PCB图)，下载推荐使用ST官方串口下载工具Flash Loader Demonstrator，固件在项目目录两个文件夹下，两个固件都可以使用，也可以自行提取固件(详细请自行搜索)，下载完成后需要将BOOT0拉低或者悬空。
![JLink_ARM_OB](https://raw.githubusercontent.com/JassyL/github_photos/master/UV4_2017-12-06_16-22-54.png)
