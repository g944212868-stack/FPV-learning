# 🚁 Drone Developer Roadmap

> 从零开始学习无人机产品开发（FPV/飞控/嵌入式），最终具备独立开发无人机产品的能力。

---

# 📖 项目介绍

本项目用于记录我从 **零基础** 学习无人机产品开发的全过程。

学习目标不是简单地完成一台无人机装机，而是深入理解：

- 无人机整体架构
- 飞控硬件设计
- 电机控制
- 飞控算法
- Betaflight源码
- STM32嵌入式开发
- 无人机产品开发流程

最终目标：

✅ 独立完成一台数字穿越机搭建

✅ 熟练使用 Betaflight

✅ 理解飞控工作原理

✅ 阅读并修改 Betaflight 源码

✅ 能参与无人机产品研发

---

# 🎯 学习目标

最终具备以下能力：

- 能独立完成无人机整机搭建
- 能独立调试飞控
- 能分析无人机硬件原理图
- 能开发STM32驱动
- 能阅读Betaflight源码
- 能实现新的飞控功能
- 能参与无人机产品开发

---

# 🗺 学习路线

```
无人机基础
        │
        ▼
电子基础
        │
        ▼
STM32开发
        │
        ▼
飞控硬件
        │
        ▼
整机搭建
        │
        ▼
Betaflight
        │
        ▼
飞控源码
        │
        ▼
飞控算法
        │
        ▼
产品开发
```

---

# 📅 项目规划

| 阶段 | 名称 | 周期 | 状态 |
|------|------|------|------|
| Phase 1 | 无人机基础 | Week1-2 | ⏳ |
| Phase 2 | 电子基础 | Week3-5 | ⏳ |
| Phase 3 | STM32开发 | Week6-10 | ⏳ |
| Phase 4 | 飞控硬件 | Week11-14 | ⏳ |
| Phase 5 | 整机装配 | Week15-18 | ⏳ |
| Phase 6 | Betaflight | Week19-22 | ⏳ |
| Phase 7 | 飞控源码 | Week23-28 | ⏳ |
| Phase 8 | 飞控算法 | Week29-32 | ⏳ |
| Phase 9 | 产品开发 | 持续 | ⏳ |

---

# 📂 Project Structure

```
FPV-learning
│
├── README.md
│
├── docs/
│   ├── 01_无人机基础
│   ├── 02_电子基础
│   ├── 03_STM32
│   ├── 04_飞控硬件
│   ├── 05_整机搭建
│   ├── 06_Betaflight
│   ├── 07_飞控源码
│   ├── 08_飞控算法
│   └── 09_产品开发
│
├── code/
│   ├── STM32
│   ├── Driver
│   ├── Betaflight
│   └── Demo
│
├── hardware/
│   ├── Datasheet
│   ├── Schematic
│   ├── PCB
│   └── BOM
│
├── images/
│
└── notes/
```

---

# 📚 Phase 1：无人机基础

## Task 01：认识无人机组成

### 学习目标

了解整架无人机各个模块的作用。

### 学习内容

- 飞控（FC）
- ESC
- 电机
- 螺旋桨
- 摄像头
- 图传（VTX）
- 接收机（Receiver）
- 电池
- GPS
- OSD

### 输出

- 绘制无人机系统框图
- 解释各模块作用

---

## Task 02：认识飞控接口

学习：

- UART
- SPI
- I2C
- USB
- ADC
- PWM
- DSHOT

完成后能够识别飞控上的所有接口。

---

## Task 03：无人机通信流程

理解整个控制流程：

```
遥控器
    │
 ELRS
    │
 Receiver
    │
 UART
    │
 Flight Controller
    │
 DSHOT
    │
 ESC
    │
 Motor
```

以及图传链路：

```
Camera
    │
 VTX
    │
 Antenna
    │
 FPV Goggles
```

---

# 📚 Phase 2：电子基础

## Task 04：万用表

学习：

- 电压
- 电阻
- 导通

实践：

测量飞控供电。

---

## Task 05：无人机供电

理解：

- VBAT
- 5V
- 3.3V
- BEC

学习供电架构。

---

## Task 06：MOSFET

理解：

为什么STM32不能直接驱动电机。

---

# 📚 Phase 3：STM32开发

## Task 07：开发环境

安装：

- CubeMX
- CubeIDE
- VSCode
- ST-Link

---

## Task 08：GPIO

点亮LED。

---

## Task 09：UART

串口输出：

Hello Drone

---

## Task 10：SPI

读取IMU数据。

---

## Task 11：PWM

PWM控制LED亮度。

---

# 📚 Phase 4：飞控硬件

## Task 12：认识飞控PCB

学习：

- MCU
- IMU
- Flash
- OSD
- BEC
- UART

---

## Task 13：飞控安装

安装飞控。

理解：

箭头方向。

---

## Task 14：ESC安装

认识：

MOS

电流路径

---

## Task 15：电机接线

理解：

三相电机工作原理。

完成：

焊接电机。

---

## Task 16：摄像头接线

连接：

Camera

VTX

---

## Task 17：ELRS接收机

完成：

接收机焊接。

---

## Task 18：首次上电

使用：

Smoke Stopper

完成首次供电测试。

---

# 📚 Phase 5：Betaflight

## Task 19

刷固件

---

## Task 20

校准IMU

---

## Task 21

配置Receiver

---

## Task 22

配置Flight Modes

---

## Task 23

测试电机方向

---

## Task 24

配置OSD

---

## Task 25

PID调试

---

# 📚 Phase 6：Betaflight源码

## Task 26

源码编译

---

## Task 27

main()

启动流程

---

## Task 28

Scheduler

任务调度

---

## Task 29

IMU驱动

---

## Task 30

PID控制

---

## Task 31

DSHOT协议

---

## Task 32

MSP协议

---

# 📚 Phase 7：飞控算法

学习：

- 欧拉角
- 四元数
- Complementary Filter
- Mahony
- Madgwick
- EKF
- PID
- FeedForward
- RPM Filter

---

# 📚 Phase 8：产品开发

## Project 01

修改OSD

---

## Project 02

增加飞行模式

---

## Project 03

开发Telemetry

---

## Project 04

开发新的Sensor Driver

---

## Project 05

设计自己的飞控PCB

---

# 🛠 当前硬件

- [x] Whoop机架
- [x] 无刷电机
- [x] 螺旋桨
- [x] 圆形AIO飞控
- [x] Flycolor FC
- [x] Flycolor ESC
- [x] 数字摄像头
- [x] 图传天线
- [x] ELRS 2.4G接收机
- [ ] 电池
- [ ] 充电器
- [ ] 遥控器（待确认）
- [ ] FPV眼镜（待确认）

---

# 📖 学习日志

| 日期 | 内容 | 状态 |
|------|------|------|
| | 初始化仓库 | ⏳ |

---

# 📌 最终目标

完成本项目后，希望达到以下能力：

- 独立开发无人机硬件
- 独立开发飞控软件
- 熟悉Betaflight源码
- 熟悉STM32嵌入式开发
- 理解无人机控制算法
- 能胜任无人机产品研发岗位

---

**Keep Flying ✈️**