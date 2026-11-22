### 你好，我是 liucoder317

嵌入式软件方向，主攻电机控制。目前在用 STM32G431 手写 FOC，做一个带 CAN 指令接口的单关节伺服驱动器。

### 项目

| 项目 | 内容 | 状态 |
|---|---|---|
| [foc-joint-servo](https://github.com/liucoder317/foc-joint-servo) | STM32G431 驱动板 + 24 V PMSM 的单关节伺服。C 手写 FOC，不用 MCSDK 和代码生成工具；电流、速度、位置三环，故障保护，CAN 指令接口 | M0 已完成；下一步 M1：互补 PWM、同步电流采样、硬件过流封波 |

### 技术栈

- **语言**：C
- **MCU**：STM32G4、STM32F1
- **外设**：GPIO、UART、TIM1 中心对齐互补 PWM 和死区、ADC 注入组同步采样、片内运放、COMP + DAC 过流比较、CAN（经典 CAN）
- **工具**：Keil MDK、STM32CubeMX、VS Code、Git、逻辑分析仪、PCAN-USB
- **在学**：FOC 电流环、速度环、位置环；FreeRTOS
