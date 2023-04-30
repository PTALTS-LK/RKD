# RP2040-based Keyboard Devkit

**这是一个基于RP2040以及CH9329键鼠芯片的，使用Kicad6.0设计的一个开源音游控制器**

你也能当成一个可编程键盘使用

**使用MicroPython作为程序主控**
<!-- 只是一个高一学生用业余时间整出来的垃圾项目罢了，PCB布线设计以及代码什么的肯定有很多问题（ -->

<details><summary>

### 预览

</summary>

![1](/Docs/PICs/IMG_1.jpg)
![2](/Docs/PICs/IMG_2.jpg)

</details>


## 特征：

  - （主要是）一个可编程键盘/4k音游控制器
    - PCB预设了SDVX的拓展板，也有只有主板的PCB
  - 使用CH9329键鼠芯片，可以模拟鼠标~~我没做~~或者键盘
  - 将RP2040的所有空闲GPIO和板载四个键使用排针引出
    - 可以用杜邦线外接按键/其他外设
    - 保留了SWD，你甚至当成一般的arm开发板进行开发
  - 键位可以方便的设置（板上Flash fat32文件系统config.json，USB大容量设备写入有概率文件损坏，建议Thonny写入）
  - 内置了宏执行器（格式请参照~~目前并不存在的~~文档）
  - 使用机械键盘键轴，可插拔（使用MX轴体）
  - 接口有MicroUSB和Type-C两种版本
  - ~~***没了***~~

## 项目文件结构
  [Docs](https://github.com/PCX-LK/RKD/tree/main/Docs) 各种文档

  [PCB](https://github.com/PCX-LK/RKD/tree/main/PCB) 当前版本的电路板Kicad设计文件

  [MPY_code](https://github.com/PCX-LK/RKD-MpyCode) Micropython主控程序

  Micropython固件可在 [RKD-MpyPort](https://github.com/PCX-LK/RKD-MpyPort) 的Release页面找到
