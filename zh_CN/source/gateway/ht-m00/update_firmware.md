# HT-M00固件升级
[English](https://heltec-automation-docs.readthedocs.io/en/latest/gateway/ht-m00/update_firmware.html)

## 摘要

本文档旨在描述如何对HT-M00进行固件升级以及将HT-M00固件覆盖的处理方法。

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

下载[HT-M00固件](https://resource.heltec.cn/download/HT-M00/firmware/M00_firmware.zip)。

打开下载好的文件，编辑"M00.bat"文件。

![](img/update_firmware/05.png)

将COM口改为HT-M00对应的COM口。

![](img/update_firmware/06.png)

修改完成后双击运行"M00.bat"，完成网关固件烧录。

```Tip:: 此固件版本为V1.2，可根据"固件升级"方法对固件进行升级。

```

