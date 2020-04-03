# LoRaWAN子频带使用示例（AU915）
[English](https://heltec-automation-docs.readthedocs.io/en/latest/general/sub_band_usage.html)
## 说明

在LoRaWAN 协议中，各国或地区都有详细的规定。这些规定包括上行和下行信道频率、带宽、占空比等。

**[LoRaWAN 1.1 Regional Parameters](https://lora-alliance.org/sites/default/files/2018-04/lorawantm_regional_parameters_v1.1rb_-_final.pdf)**

以AU915为例：

![](img/sub-band_usage/01.png)



让我们看我们的代码: (在LoRaWan_APP.cpp中)

![](img/sub-band_usage/02.png)

下面是为AU915定义的所有LoRaWAN 协议通道的5个阵列。在channelsMaskTemp[0]中，0x00FF表示使用前0-7个信道，它们是915.2MHz、915.4MHz、915.6MHz…916.6MHz。当您将该值设置为0xFF00时，意味着上载通道更改为8-15，它们是916.8MHz、917.0MHz…918.2MHz。更多细节。。。见下图：

![](img/sub-band_usage/03.png)

TTN仅对AU915使用第二子带（信道8至15和65）：

https://www.thethingsnetwork.org/docs/lorawan/frequency-plans.html

![](img/sub-band_usage/04.png)

## 使用方法

一般来说，我们只需要更改"channelsMaskTemp[0]=0xFF00"，然后上行链路频率将更改为支持TTN。

你的LoRa 网关的监听频率必须与TTN服务器相同。它在网关的“gloable_conf.json”文件中定义。