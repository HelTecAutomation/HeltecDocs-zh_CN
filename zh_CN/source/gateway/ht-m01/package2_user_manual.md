# HT-M01套餐二使用手册

[English]()

## 摘要

用户购买HT-M01套餐二后，我们将会对网关和树莓派进行相应软件配置，用户拿到网关和树莓派后只需在相应服务器新建对应网关和节点后即可正常使用。默认使用[HelTec服务器](http://cloud.heltec.org/)，用户需要使用HelTec账号登录，可在官网注册。用户也可修改服务器地址以使用其他服务器。

&nbsp;

## 查看及修改网关信息

- 如下图所示给网关与树莓派通电，其中"1"为串口线，"2"为电源线。如果直接上电使用，不修改树莓派配置，则只需连接2号电源线。

![](img/package2_user_manual/01.png)

- 通过串口工具(如”[putty](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)")打开树莓派对应串口，可以看到串口会打印树莓派的启动日志信息。并通过默认用户名和密码登录(在Linux系统中，通过命令行输入密码的过程是看不到任何变化的)。

```shell
用户名：pi
密码：raspberry
```

![](img/package2_user_manual/02.png)

- 网关ID可在"/home/pi/lora/packet_forwarder/lora_pkt_fwd/local_conf.json"中查看。

![](img/package2_user_manual/03.png)

- 网关ID和服务器地址可在"/home/pi/lora/packet_forwarder/lora_pkt_fwd/ global_conf.json"中修改。

![](img/package2_user_manual/04.png)

- 在相应的服务器中新建相应的网关和节点后就能查看上下行信息。如果使用默认的[HelTec服务器](http://cloud.heltec.org/)，需要使用HelTec账号登录，可在官网注册。

