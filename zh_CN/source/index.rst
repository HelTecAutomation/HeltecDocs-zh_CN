Heltec Automation文档页
=======================
`English <https://heltec-automation-docs.readthedocs.io/en/latest/index.html>`_

这些是 `Heltec Automation <https://heltec.org>`_ 产品的文档。
   
==================  ==================  ==================
|CubeCell|_         |ESP32+LoRa|_       |STM32+LoRa|_
------------------  ------------------  ------------------
`CubeCell`_         `ESP32+LoRa`_       `STM32+LoRa`_
------------------  ------------------  ------------------
|ESP32+Arduino|_    |ESP8266+Arduino|_  |General Docs|_
------------------  ------------------  ------------------
`ESP32+Arduino`_    `ESP8266+Arduino`_  `General Docs`_
==================  ==================  ==================

.. |CubeCell| image:: img/01.png
.. _CubeCell: cubecell/index.html

.. |ESP32+LoRa| image:: img/02.png
.. _ESP32+LoRa: esp32/index.html

.. |STM32+LoRa| image:: img/03.png
.. _STM32+LoRa: stm32/index.html

.. |ESP32+Arduino| image:: img/04.png
.. _ESP32+Arduino: esp32+arduino/index.html

.. |ESP8266+Arduino| image:: img/05.png
.. _ESP8266+Arduino: esp8266+arduino/index.html

.. |General Docs| image:: img/06.png
.. _General Docs: general/index.html


.. toctree::
   :hidden:
   :caption:
   
   简体中文 <https://heltec-automation.readthedocs.io/zh_CN/latest/index.html>

.. toctree::
   :hidden:
   :caption: LORA GATEWAY
   
   gateway/index
   gateway/ht-m01/index
   gateway/ht-m02/index
   常见问题 <gateway/frequently_asked_questions>
   
.. toctree::
   :hidden:
   :caption: CubeCell

   cubecell/index
   快速入门 <cubecell/quick_start>
   cubecell/lorawan/index
   AT命令列表 <https://docs.heltec.cn/download/cubecell/CubeCell_Series_AT_Command_User_Manual_V0.2.pdf>
   cubecell/htcc-am01/index
   cubecell/htcc-ab01/index
   cubecell/htcc-ac01/index
   常见问题 <cubecell/frequently_asked_questions>

.. toctree::
   :hidden:
   :caption: ESP32 + LoRa

   esp32/index
   快速入门 <esp32/quick_start>
   esp32/lorawan/index
   最大距离测试 <esp32/distance_test>
   esp32/wifi_lora_32/index
   esp32/wireless_stick/index
   esp32/wireless_stick_lite/index
   esp32/wireless_shell/index
   常见问题 <esp32/frequently_asked_questions>

.. toctree::
   :hidden:
   :caption: STM32 + LoRa

   stm32/index
   快速入门 <stm32/quick_start>
   stm32/lorawan/index
   stm32/lora_node_151/index
   stm32/turtle_board/index
   常见问题 <stm32/frequently_asked_questions>

.. toctree::
   :hidden:
   :caption: ESP32 + Arduino
   
   esp32+arduino/index
   快速入门 <esp32+arduino/quick_start>
   esp32+arduino/wifi_kit_32/index
   常见问题 <esp32+arduino/frequently_asked_questions>
   
.. toctree::
   :hidden:
   :caption: ESP8266 + Arduino

   esp8266+arduino/index
   快速入门 <esp8266+arduino/quick_start>
   esp8266+arduino/wifi_kit_8/index
   常见问题 <esp8266+arduino/frequently_asked_questions>

.. toctree::
   :hidden:
   :caption: General Docs

   general/index
   怎样安装Git和Arduino <general/how_to_install_git_and_arduino>
   建立串行连接 <general/establish_serial_connection>
   LoRaWAN子频带使用示例 <general/sub_band_usage>
   订阅MQTT消息 <general/subscribe_mqtt_messages>
   解码LoRaWAN有效载荷 <general/decode_payload>
   怎样配置树莓派 <general/how_to_config_raspberry_pi>
   获取受限的技术资源 <general/view_limited_technical_data>