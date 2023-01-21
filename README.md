# RP2040-based Keyboard Devkit

**这是一个基于RP2040以及CH9329键鼠芯片的，使用Kicad6.0设计的一个开源音游控制器**

**使用MicroPython作为程序主控**

_~~只是一个高一学生用业余时间整出来的垃圾项目罢了，PCB布线设计以及代码什么的肯定有很多问题（~~_

<details><summary>

### 预览

</summary>

![1](/Docs/PICs/IMG_1.jpg)
![2](/Docs/PICs/IMG_2.jpg)

</details>


## 特征：

  - （主要是）一个4k音游控制器
  - 使用CH9329键鼠芯片，可以模拟鼠标~~我没做~~或者键盘
  - 将RP2040的几乎所有引脚引出，可自行外接按键
    - PCB预设了SDVX的拓展板
  - 键位可以方便的设置（板上Flash fat32文件系统config.json）
  - 内置了宏执行器（格式请参照文档）
  - 使用机械键盘键轴，可插拔（使用MX轴体）
  - 仍在使用~~极为先进~~早就落伍的MicroUSB接口
  - ~~***没了***~~

## 项目文件结构
  [Docs](https://github.com/PCX-LK/RKD/tree/main/Docs) 各种文档

  [PCB](https://github.com/PCX-LK/RKD/tree/main/PCB) 当前版本的电路板Kicad设计文件

  [MPY_code](https://github.com/PCX-LK/RKD/tree/main/MPY_code) Micropython主控程序

  Micropython固件可在 [RKD-MpyPort](https://github.com/PCX-LK/RKD-MpyPort) 的Release页面找到
