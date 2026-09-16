# STM32多舵机机械臂控制系统

## 项目简介
基于STM32F103 + FreeRTOS + CAN总线的多自由度机械臂控制系统，实现多关节独立角度控制与闭环调速。

## 硬件平台
- 主控：STM32F103C8T6
- 通信：CAN总线（1Mbps）
- 执行器：MG996R舵机 × 3
- 传感器：MPU6050、编码器电机

## 软件架构
- FreeRTOS多任务：CanRxTask / ControlTask / FaultMonitorTask
- PID闭环控制（增量式+积分分离）
- CAN总线仲裁与心跳检测

## 功能演示
附件视频

## 如何编译
1. 用STM32CubeMX打开`.ioc`文件
2. 用Keil MDK打开工程，编译下载

## 联系方式
- 邮箱：18572127551@163.com
