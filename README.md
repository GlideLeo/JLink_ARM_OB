

# JLink_ARM_OB(Type-C)
![](https://img.shields.io/badge/Version-1.4-brightgreen.svg)    ![](https://img.shields.io/badge/license-CC4.0-brightgreen.svg)
* Author: [DataSheep](https://github.com/JassyL/DAP_Link)
* Version: 1.4
* Update: 2018.11.06

# Description

JLink-OB (STM32F072C8) is a JLink_OB download emulator based on **STM32F072C8T6**. It has the same functions as J-Link and ST-Link, and **supports virtual serial port** for easy debugging. This version is based on the [X893/CMSIS-DAP](https://github.com/x893/CMSIS-DAP) modification. On-board 5V and 3.3V output, suitable for a variety of Cotex-M core microcontrollers.

This version of JLink_ARM_OB uses STM32F072C8 internal oscillations, eliminating the need for an external crystal, which make a smaller PCB area.

JLink-OB (STM32F072C8)是基于STM32F072C8T6的一款JLink_OB下载仿真器，具有J-Link、ST-Link等相同功能，**并且支持虚拟串口**，方便调试。本版本基于[X893/CMSIS-DAP](https://github.com/x893/CMSIS-DAP)修改。板载5V和3.3V输出，适合各种Cotex-M内核单片机。

此版本JLink_ARM_OB使用STM32F072C8内部震荡，省去了外部晶振，PCB面积更小。

# License

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/deed.zh"><img alt="知识共享许可协议" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />

This work was produced by DataSheep and licensed under a Creative Commons Attribution-Share Alike 4.0 International License Agreement.

本作品由[DataSheep](https://github.com/JassyL/DAP_Link)制作，采用<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/deed.zh">知识共享署名-相同方式共享 4.0 国际许可协议</a>进行许可。

# Photos
#### PCB
![](http://qiniu.youngafar.com/dap3.png-sy)

#### Photos during test

![JLink_ARM_OB](https://raw.githubusercontent.com/JassyL/github_photos/master/tset_1.png "测试照片")

![](http://qiniu.youngafar.com/20181105183437.png-syg)

# Instructions for use

This version does not have the SW download interface, it can be programed through the serial port, the BOOT0 on the back must be connected with 3.3v before programing (see PCB diagram), you can use the ST official serial programing tool Flash Loader Demonstrator, firmware in the project directory. After the download is complete, you need to lower BOOT0 or leave it empty.

此版本没有留SW下载接口，可通过串口下载，下载前将背面BOOT0接高(详见PCB图)，下载推荐使用ST官方串口下载工具Flash Loader Demonstrator，固件在项目目录文件夹下，下载完成后需要将BOOT0拉低或者悬空。
![JLink_ARM_OB](https://raw.githubusercontent.com/JassyL/github_photos/master/UV4_2017-12-06_16-22-54.png)

# Update for usb Type-C interface

For ease of use, the USB Type-C interface has been updated with the advantage of being able to plug in and out and eliminating the need to prepare an extra micro USB cable. For details, please refer to the article: [Upgrade Type-C Interface](https://www.datasheep.cn/2018/11/05/DAP_Link_3/)

为了方便使用，更新了USB Type-C接口，好处是可以正反插，并且不用再准备一根多余的micro USB数据线。详细内容可以参考文章：[升级Type-C接口](https://www.datasheep.cn/2018/11/05/DAP_Link_3/)。