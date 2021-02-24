[[英文]](README.md)

这个工程是使用涂鸦SDK开发的。涂鸦SDK可以让你快速地开发可以连接和控制有很多设备的智能场景的品牌APP，了解更多，请访问[涂鸦开发者](https://iot.tuya.com).

# 简介
* 从板载的SHT30温湿度传感器获取温湿度信息
* 在0.96"OLED显示这些信息
* 上传这些信息到涂鸦云平台使我能在涂鸦APP中看到温湿度信息

# 视频
在我的[立创开源项目](https://oshwhub.com/baobaoa/wu-lian-wang-qi-xiang-tai-657332a)中
# 硬件部分
WBR3D WiFi 模块

SHT30 温湿度传感器

SSD1306 0.96"OLED 屏幕

STM32G431CBT6 单片机

[PCB 链接](https://oshwhub.com/baobaoa/wu-lian-wang-qi-xiang-tai-657332a)
# 软件
涂鸦提供的MCU SDK

STM32 CubeMX with HAL

源码在"source"文件夹内

# 接下来要做的事
这是我第一块使用涂鸦模组的板子。而且这确实暴露出一些问题来
* 使用的LDO发热过于严重以至于影响到了温度传感器，大约2到3度
* 使用的MCU有一些昂贵。尽管我购得此MCU仅10元，使用这么一颗高性能的MCU来做这么简单的事情仍然是不合适的
* OLED屏幕的固定方式（使用排母和排针连接）是较为不可靠的
* USB串口芯片和Flash芯片可能是没有必要的
