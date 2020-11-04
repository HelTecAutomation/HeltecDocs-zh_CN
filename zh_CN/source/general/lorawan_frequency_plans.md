# LoRaWAN频率计划

[English](https://heltec-automation-docs.readthedocs.io/en/latest/general/lorawan_frequency_plans.html)

## 摘要

这是LoRaWAN频率计划的列表。 这些频率计划基于LoRaWAN区域参数文档中指定的内容。 要了解您所在国家/地区使用的频率计划，请参阅[按国家/地区列表列出的频率计划](https://heltec-automation.readthedocs.io/zh_CN/latest/general/lorawan_frequency_plans_by_country.html)。

&nbsp;

## EU863-870

- Uplink:

1. **868.1** - SF7BW125 to SF12BW125
2. **868.3** - SF7BW125 to SF12BW125 and SF7BW250
3. **868.5** - SF7BW125 to SF12BW125
4. **867.1** - SF7BW125 to SF12BW125
5. **867.3** - SF7BW125 to SF12BW125
6. **867.5** - SF7BW125 to SF12BW125
7. **867.7** - SF7BW125 to SF12BW125
8. **867.9** - SF7BW125 to SF12BW125
9. **868.8** - FSK

- Downlink:
  - Uplink channels 1-9 (RX1)
  - **869.525** - SF9BW125 (RX2)

```Tip:: 请注意，物联网在欧洲对RX2使用非标准SF9BW125数据速率。 如果您的设备使用OTAA，则它们在加入时将自动进行配置。 如果您的设备使用ABP，则需要将此RX2数据速率编程到设备中。

```

&nbsp;

## EU433

尚无频率计划。

&nbsp;

## US902-928

在美国，加拿大和南美使用

- Uplink:

1. **903.9** - SF7BW125 to SF10BW125
2. **904.1** - SF7BW125 to SF10BW125
3. **904.3** - SF7BW125 to SF10BW125
4. **904.5** - SF7BW125 to SF10BW125
5. **904.7** - SF7BW125 to SF10BW125
6. **904.9** - SF7BW125 to SF10BW125
7. **905.1** - SF7BW125 to SF10BW125
8. **905.3** - SF7BW125 to SF10BW125
9. **904.6** - SF8BW500

- Downlink:

1. **923.3** - SF7BW500 to SF12BW500 (RX1)
2. **923.9** - SF7BW500 to SF12BW500 (RX1)
3. **924.5** - SF7BW500 to SF12BW500 (RX1)
4. **925.1** - SF7BW500 to SF12BW500 (RX1)
5. **925.7** - SF7BW500 to SF12BW500 (RX1)
6. **926.3** - SF7BW500 to SF12BW500 (RX1)
7. **926.9** - SF7BW500 to SF12BW500 (RX1)
8. **927.5** - SF7BW500 to SF12BW500 (RX1)
9. **923.3** - SF12BW500 (RX2)

&nbsp;

## CN470-510

在中国使用

- Uplink:

1. **486.3** - SF7BW125 to SF12BW125
2. **486.5** - SF7BW125 to SF12BW125
3. **486.7** - SF7BW125 to SF12BW125
4. **486.9** - SF7BW125 to SF12BW125
5. **487.1** - SF7BW125 to SF12BW125
6. **487.3** - SF7BW125 to SF12BW125
7. **487.5** - SF7BW125 to SF12BW125
8. **487.7** - SF7BW125 to SF12BW125

- Downlink:

1. **506.7** - SF7BW125 to SF12BW125 (RX1)
2. **506.9** - SF7BW125 to SF12BW125 (RX1)
3. **507.1** - SF7BW125 to SF12BW125 (RX1)
4. **507.3** - SF7BW125 to SF12BW125 (RX1)
5. **507.5** - SF7BW125 to SF12BW125 (RX1)
6. **507.7** - SF7BW125 to SF12BW125 (RX1)
7. **507.9** - SF7BW125 to SF12BW125 (RX1)
8. **508.1** - SF7BW125 to SF12BW125 (RX1)
9. **505.3** - SF12BW125 (RX2)

&nbsp;

## AU915-928

- Uplink:

1. **916.8** - SF7BW125 to SF12BW125
2. **917.0** - SF7BW125 to SF12BW125
3. **917.2** - SF7BW125 to SF12BW125
4. **917.4** - SF7BW125 to SF12BW125
5. **917.6** - SF7BW125 to SF12BW125
6. **917.8** - SF7BW125 to SF12BW125
7. **918.0** - SF7BW125 to SF12BW125
8. **918.2** - SF7BW125 to SF12BW125
9. **917.5** - SF8BW500

- Downlink:

1. **923.3** - SF7BW500 to SF12BW500 (RX1)
2. **923.9** - SF7BW500 to SF12BW500 (RX1)
3. **924.5** - SF7BW500 to SF12BW500 (RX1)
4. **925.1** - SF7BW500 to SF12BW500 (RX1)
5. **925.7** - SF7BW500 to SF12BW500 (RX1)
6. **926.3** - SF7BW500 to SF12BW500 (RX1)
7. **926.9** - SF7BW500 to SF12BW500 (RX1)
8. **927.5** - SF7BW500 to SF12BW500 (RX1)
9. **923.3** - SF12BW500 (RX2)

```Tip:: Note that The Things Network uses 2nd Sub-Band only (channels 8 to 15 and 65). You’ll need to program the specific channels into the devices.

```

&nbsp;

## AS923

根据国家/地区使用两个频率计划。 OTAA设备使用两个公共通道：923.2MHz和923.4MHz。 成功加入后，他们将获得其他渠道。

### AS920-923 (“AS1”)

Used in Japan, Malaysia, Singapore

- Uplink:

1. **923.2** - SF7BW125 to SF12BW125
2. **923.4** - SF7BW125 to SF12BW125
3. **922.2** - SF7BW125 to SF12BW125
4. **922.4** - SF7BW125 to SF12BW125
5. **922.6** - SF7BW125 to SF12BW125
6. **922.8** - SF7BW125 to SF12BW125
7. **923.0** - SF7BW125 to SF12BW125
8. **922.0** - SF7BW125 to SF12BW125
9. **922.1** - SF7BW250
10. **921.8** - FSK

-  Downlink:
  - Uplink channels 1-10 (RX1)
  - **923.2** - SF10BW125 (RX2)

### AS923-925 (“AS2”)

用于文莱，柬埔寨，香港，印度尼西亚，老挝，台湾，泰国，越南

- Uplink:

1. **923.2** - SF7BW125 to SF12BW125
2. **923.4** - SF7BW125 to SF12BW125
3. **923.6** - SF7BW125 to SF12BW125
4. **923.8** - SF7BW125 to SF12BW125
5. **924.0** - SF7BW125 to SF12BW125
6. **924.2** - SF7BW125 to SF12BW125
7. **924.4** - SF7BW125 to SF12BW125
8. **924.6** - SF7BW125 to SF12BW125
9. **924.5** - SF7BW250
10. **924.8** - FSK

- Downlink:
  - Uplink channels 1-10 (RX1)
  - **923.2** - SF10BW125 (RX2)

&nbsp;

## KR920-923

- Uplink:

1. **922.1** - SF7BW125 to SF12BW125
2. **922.3** - SF7BW125 to SF12BW125
3. **922.5** - SF7BW125 to SF12BW125
4. **922.7** - SF7BW125 to SF12BW125
5. **922.9** - SF7BW125 to SF12BW125
6. **923.1** - SF7BW125 to SF12BW125
7. **923.3** - SF7BW125 to SF12BW125
8. *none*

- Downlink:
  - Uplink channels 1-7
  - **921.9** - SF12BW125 (RX2; SF12BW125 might be changed to SF9BW125)

&nbsp;

## IN865-867

- Uplink:

1. **865.0625** - SF7BW125 to SF12BW125
2. **865.4025** - SF7BW125 to SF12BW125
3. **865.9850** - SF7BW125 to SF12BW125

- Downlink:
  - Uplink channels 1-3 (RX1)
  - **866.550** - SF10BW125 (RX2)

&nbsp;

## 相关资源

- [频率计划](https://www.thethingsnetwork.org/docs/lorawan/frequency-plans.html)