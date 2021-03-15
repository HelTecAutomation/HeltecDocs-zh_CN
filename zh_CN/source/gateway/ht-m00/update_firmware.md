# HT-M00固件升级
[English](https://heltec-automation-docs.readthedocs.io/en/latest/gateway/ht-m00/update_firmware.html)

## 摘要

本文档旨在描述如何对HT-M00进行固件升级以及将HT-M00固件覆盖的处理方法。

```Tip:: 由于HT-M00固件版本V1.8更新了网关激活码算法。 因此，从V1.7及以下版本升级到V1.8及以上版本需要重新激活HT-M00网关。 请将网关ESP32芯片ID发送至“ support@heltec.cn”，我们将为您重新计算激活码并将其上传至服务器。

```

&nbsp;

## 固件升级

下载[HT-M00相应升级固件](https://resource.heltec.cn/download/HT-M00/firmware)。

![](img/update_firmware/01.png)

通过连接HT-M00的WiFi进入HT-M00网关配置界面(可参考[HT-M00快速入门](https://heltec-automation.readthedocs.io/zh_CN/latest/gateway/ht-m00/qucik_start.html))，再点击"Firmwaer Update"。

![](img/update_firmware/02.png)

点击"Select firmware"选择下载好的相应升级固件，点击"Update"进行升级。

![](img/update_firmware/03.png)

升级完成后，将弹出相应提示并重启网关。

![](img/update_firmware/04.png)

&nbsp;

## HT-M00固件覆盖处理方法

下载[HT-M00固件](https://resource.heltec.cn/download/HT-M00/firmware/M00_firmware_V1.4.zip)。

打开下载好的文件，编辑"M00.bat"文件。

![](img/update_firmware/05.png)

将COM口改为HT-M00对应的COM口。

![](img/update_firmware/06.png)

修改完成后双击运行"M00.bat"，完成网关固件烧录。

M00重新刷新固件后串口打印显示没有激活的情况。请参考这篇帖子:

[http://community.heltec.cn/t/solved-restoring-esp32-chip-license-to-ht-m00-flash-memory/2676](http://community.heltec.cn/t/solved-restoring-esp32-chip-license-to-ht-m00-flash-memory/2676)

```Tip:: 此固件版本为V1.4，可根据"固件升级"方法对固件进行升级。

```

