**功率测量**
==================

:link_to_translation:`en:[English]`

本示例演示了如何使用BL0937功率测量芯片来检测电压、电流、有功功率和能耗等电气参数。使用 FreeRTOS 在ESP32上实现,展示了如何配置BL0937功率测量芯片并与开发芯片连接。该示例初始化功率测量系统、获取各种参数并定期记录。

适配列表
-----------------------

+--------+--------------------------------------------------+---------+---------------------------------------------------------------------------------------------------------------------+------------+
|  名称  |                       功能                       |  供应商 |                                                        规格书                                                       | 硬件抽象层 |
+========+==================================================+=========+=====================================================================================================================+============+
| BL0937 | 检测电量参数，例如电压、电流以及功率和消耗的电量 | BELLING | `BL0937 Datasheet <https://www.belling.com.cn/media/file_object/bel_product/BL0937/datasheet/BL0937_V1.02_en.pdf>`_ |      x     |
+--------+--------------------------------------------------+---------+---------------------------------------------------------------------------------------------------------------------+------------+


API 参考
--------------------

The following API implements hardware abstraction for power measure. Users can directly call this layer of code to write sensor applications.

.. include-build-file:: inc/power_measure.inc