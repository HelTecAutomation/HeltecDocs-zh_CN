# Wifi Kit 32  Hardware Update Logs

## V1

![](img/hardware_update_log/01.png)

- First release
- 2017-6-1 public sale

- [Pin out diagram for V1](http://resource.heltec.cn/download/WiFi_Kit_32/WIFI%20Kit%2032_pinoutDiagram_V1.pdf)
- [Schematic diagram for V1](http://resource.heltec.cn/download/WiFi_Kit_32/WIFI_Kit_32_Schematic_diagram_V1.PDF)

&nbsp;

## V2

![](img/hardware_update_log/02.png)

- 20 public sale
- 修复充电状态（橙色LED）闪烁问题；;
- 4MB（32M位）FLASH 升级到8MB（64M位）FLASH ；
- 更好的2.4GHz天线设计和阻抗匹配；;
- 基本低功耗设计（深度睡眠800uA）；
- 增加电池电量检测电路。使用ADC2_4（GPIO 13）读取电池电压；
- 添加Vext电源输出引脚，用户可以使用该引脚驱动一些外部设备（传感器、电机等），当系统需要进入深度睡眠模式时，Vext可以关闭。**此引脚由GPIO21控制，例如：**
- Turn ON: `digitalWrite(21, LOW);`
  
- Turn OFF: `digitalWrite(21, HIGH);`
- 电路优化，系统更稳定；
- 更好的电源管理系统设计。
- [Pin out diagram for V2](http://resource.heltec.cn/download/WiFi_Kit_32/WIFI_Kit_32_pinoutDiagram_V2.pdf);
- [Schematic diagram for V2](http://resource.heltec.cn/download/WiFi_Kit_32/WIFI_Kit_32_Schematic_diagram_V2.pdf);

&nbsp;

## V2.1

- 2019-10 public sale?
- 修复电池电压读数无法与Wi-Fi一起工作，将电池电压读数引脚更改为GPI37（使用ADC1_1），请参阅以下示例：[ADC_Read_Voltage/Battery_power](https://github.com/HelTecAutomation/Heltec_ESP32/blob/master/examples/ESP32/ADC_Read_Voltage/Battery_power/Battery_power.ino)。
- [Pin out diagram for V2.1]();
- [Schematic diagram for V2.1]();



