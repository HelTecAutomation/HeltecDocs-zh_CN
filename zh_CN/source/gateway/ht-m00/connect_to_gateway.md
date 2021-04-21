# 将节点连接到HT-M00

[English](https://heltec-automation-docs.readthedocs.io/en/latest/gateway/ht-m00/connect_to_gateway.html)

## 摘要

本文旨在描述如何将节点连接到[HT-M00 网关](https://heltec.org/project/ht-m00/)，从而促进LoRa设备的二次开发和快速部署。HT-M00为双通道网关，为保证节点与网关通信良好，需使节点使用的通道与HT-M00网关的通道相对应。本文档以CN470为例。

在所有操作之前，请确保节点和HT-M00运行良好。如果没有，请参考[HT-M00快速入门](https://heltec-automation.readthedocs.io/zh_CN/latest/gateway/ht-m00/quick_start.html)文档。

```Tip:: 如果节点通道多于网关通道且将网关通道包含在内，那么只有当节点通道与网关通道匹配时才能入网，如果节点通道不包含网关通道，那么节点不能入网。

```

&nbsp;

## 通道频率

![](img/connect_to_gateway/01.png)

CN470从470.3MHz到489.3MHz共对应96个通道，频率每增加200kHz，通道编码增加1，即：

freq=470.3+0.2*N（N为通道编码 0-95）

让我们看看代码: (在LoRaWAN对应的`.ino`文件中)

CubeCell系列可参考"LoRaWAN",ESP32系列可参考"OTTA"。

![](img/connect_to_gateway/02.png)

这是为CN470定义的所有LoRaWAN 协议通道的6个阵列。在userChannelsMask[0]中，0x00FF表示使用前0-7个通道，它们是470.3MHz、470..5MHz、470.7MHz…471.7MHz。将十六进制FF转换为二进制是11111111，8个1从低位到高位分别对应前0-7个通道，即最后一个1对应通道0，第一个1对应通道7。当您修改"userChannelsMask[0]=0x0001"时，意味着通道更改为0，它是470.3MHz；修改"userChannelsMask[0]=0x0080"时，意味着通道更改为7，它是471.7MHz。当修改"userChannelsMask[0]=0xFF00"时，意味着通道更改为8-15，它们是471.9MHz、472.1MHz、472.3MHz...473.3MHz。

&nbsp;

## 使用方法

HT-M00的网页配置界面如下。

![](img/connect_to_gateway/03.png)

在HT-M00的配置界面中，会配置网关的两个通道频率，我们需要使节点使用的通道与这两个通道对应，即在相应程序中修改通道掩码。

以CubeCell系列为例：

![](img/connect_to_gateway/04.png)

如果网关配置通道为471.9MHz和472.1MHz，则使用9，10通道。在LoRaWAN程序中，需修改"userChannelsMask[0]=0x0300"。