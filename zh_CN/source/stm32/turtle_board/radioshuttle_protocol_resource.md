# 无线电传输协议资源
[English](https://heltec-automation-docs.readthedocs.io/en/latest/stm32/turtle_board/radioshuttle_protocol_resource.html)

## 无线传输协议

- **点对点LoRa 无线协议软件**

  标准的**LoRaWAN**协议效率低，不支持直接的节点间通信，而且对于许多应用程序来说太昂贵和复杂。无线电中继可以在简单的LoRa 模块之间高效、安全地发送信息。

- **安全信息传输**

  最多232字节用户数据，接收将被确认，丢失的数据将自动重发

- **空中交通管制**

  只有当该信道上没有激活的LoRa 信号时，节点才会发送。站点创建自动网络计划，定义允许哪些节点和站点通信以及何时通信。（计划中）

- **优化的协议**

  - 110 ms内的消息传送（SF7，125 kHz，提供免费信道）
  - 消息只需要2 x 12字节（协议开销）
  - 窄带宽允许更长的范围
  - 发射功率自动调整，节能降耗
  
- **支持多个MCU开发板**

  - The [Turtle](https://www.radioshuttle.de/en/turtle-en/turtle-board-en/) board
  - The [ECO Power](https://www.radioshuttle.de/en/esp32-eco-power-en/esp32-eco-power-board-en/) board
  - The [LongRa](https://www.radioshuttle.de/en/longra-en/board-en/) board

- **支持多个系统**

  - Arduino, Arduino Zero or newer
  - ARM Mbed OS, supported MCUs (e.g. STM32L0, STM32L4)
  - Linux (Raspberry PI/Orange PI planned)

  了解更多有关无线电传输协议的信息，请点击:[The RadioShuttle Wireless Protocol](https://www.radioshuttle.de/en/radioshuttle-en/protocol/).

  &nbsp;

## RadioShuttle STM32 Utility

“RadioShuttle STM32 Utility”是一个特殊的实用程序，它可以使用DFU协议通过USB轻松地将软件上载到RadioShuttle STM32兼容板或从中下载软件。该实用程序可以从Mac、Windows和Linux的命令行使用，也可以在Mac和Windows计算机的GUI中使用。软件可上传至/下载自STM32 MCU。它被设计用于在制造过程中获得有效许可证（代码）的无线电换向兼容板。

- **系统要求**

  - **Windows:** Windows 7 or higher
  - **Mac:** macOS 10.9 or higher
  - **Linux:** Linux kernel 2.6.16 or higher,glibc 2.4 or higher

  了解更多有关RadioShuttle STM32 Utility 信息请点击: [RadioShuttle STM32 Utility](https://www.radioshuttle.de/en/turtle-en/radioshuttle-stm32-utility-en/)
  

