目录
====
`English <https://heltec-automation-docs.readthedocs.io/en/latest/cubecell/index.html>`_

我们认为 `“CubeCell系列” <https://heltec.org/cubecell>`_ 是最好的LoRaWAN节点应用的选择。以下是一些关键特征：

-  与Arduino开发环境完全兼容；
-  基于超低功耗设计，即使在RTC时钟运行的情况下，在深度睡眠模式下也能达到3.5μA；
-  LoRa信号输出功率范围0~22（±1）dBm;
-  尽管具有当前最先进的技术，但价格低廉；
-  通过使用集成加密算法来使克隆的固件不起作用以保护您的投资；
-  基于成熟的技术 -- 新的ASR650x，是将PSoC4000和SX1262组合成一个芯片，将整体尺寸进一步缩小；
-  支持太阳能电池板；
-  LoRaWAN协议支持；
-  支持AT命令;
-  在LoRaWAN相关的例程中，有一个合理的时间表规划。

.. tip::

   例如，一个应用程序需要每10分钟向服务器发送一次数据，然后在一个周期内，只有大约1秒处于发送状态，其他9分59秒处于深度睡眠低功耗状态。


.. toctree::
    :maxdepth: 2
    
    快速入门 <quick_start>
    LoRaWAN <lorawan/index>
    AT命令列表 <https://resource.heltec.cn/download/CubeCell/AT_Command_list_zh-CN/CubeCell_Series_AT_Command_User_Manual_zh_CN_V0.6.pdf>  
    CubeCell开发板 <dev-board/index>
    CubeCell胶囊传感器 <capsule-sensor/index>
    CubeCell模块 <module/index>
    常见问题 <frequently_asked_questions>

相关官方资源
------------

- `ASR650x - Arduino repository <https://github.com/HelTecAutomation/ASR650x-Arduino>`_;
- `CubeCell简介页面 <https://heltec.org/cubecell/>`_。

