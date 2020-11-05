#  	LoRa节点连接到单/双通道网关
[English](https://heltec-automation-docs.readthedocs.io/en/latest/general/connect_to_single_channel_gateway.html)

## 摘要

本文旨在描述如何将节点连接到少于8个通道的非标准网关(例如单通道网关和[Heltec HT-M00双通道网关](https://heltec.org/project/ht-m00))。 节点和网关之间成功通信的关键：**网关和节点之间的发送/监听频率必须匹配！**

```Tip:: 如果节点通道多于网关通道且将网关通道包含在内，那么只有当节点通道与网关通道匹配时才能入网，如果节点通道不包含网关通道，那么节点不能入网。

```

&nbsp;

## 通信通道和频率

在LoRaWAN协议中，详细定义了每个频段的上行链路和下行链路频率。 这些使用的频率称为通道。 作为参考，我们在协议文档中截取了CN470-510通道定义的描述。

![](img/connect_to_single_channel_gateway/01.png)

CN470对应于从470.3MHz到489.3MHz的总共96个通道。 每增加200kHz频率，信道代码将增加1，即：

`freq(MHz)=470.3+0.2*N`

在loramac-node的代码中，`userChannelsMask` 数组中的内容对应于通信通道。 设置为1表示该通道已启用。

在[Heltec ESP32 LoRa](https://heltec.org/proudct_center/lora/lora-node/)和[CubeCell](https://heltec.org/proudct_center/lora/cubecell/)示例代码中，我们将`ChannelsMask`定义移到了`.ino`文件中。

![](img/connect_to_single_channel_gateway/02.png)

在默认定义中，已启用通道0〜7，并且如果节点使用频带CN470，则意味着节点发送日期将使用470.3〜471.7 MHz，而下行消息将使用500.3〜501.7 MHz。

如果代码变成这个，那将是什么通道？

`uint16_t userChannelsMask [6] = {0x0000,0xFFF0,0x0000,0x0000,0x0000,0x0000};`

答案是**21至32通道**。

&nbsp;

## 使用方法

一般来说，要将节点连接到单/双通道网关，我们需要使节点使用的通道与单/双通道网关的通道相对应！

- 示例1-连接到[Heltec HT-M00双通道网关](https://heltec.org/project/ht-m00/)

如果将HT-M00设置为472. 1和472.3（通道10、11），则“ ChannelsMask”应为：

`uint16_t userChannelsMask [6] = {0x0600,0x0000,0x0000,0x0000,0x0000,0x0000};`

- 示例2-连接到单通道网关

单通道网关设置为470.7 MHz（通道3），`ChannelsMask`应该是；

`uint16_t userChannelsMask [6] = {0x0004,0x0000,0x0000,0x0000,0x0000,0x0000};`

## 相关资源

- [固定前导码长度以适应HT-M00双通道网关](https://heltec-automation.readthedocs.io/zh_CN/latest/gateway/frequently_asked_questions.html#ht-m00)