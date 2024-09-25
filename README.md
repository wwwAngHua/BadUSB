# Raspberry Pi Pico Bad USB

如何使用 Raspberry Pi Pico 制作 Bad USB 模拟键盘执行输入？！

1. 首先按住树莓派 Raspberry Pi Pico BOOTSEL 键进入 bootloader 模式；这时系统就会多出一个磁盘。

2. 进入磁盘，将 adafruit-circuitpython-raspberry_pi_pico-en_US-8.0.0.uf2 固件文件拷贝到该磁盘中（树莓派会自动断开 2 秒）。

3. 删除磁盘中的所有文件，并把 files 目录下的所有文件拷贝至磁盘中。

4. 编辑磁盘中的 payload.dd 文件，输入你想摸你的键盘指令。

5. 重新插入 Raspberry Pi Pico 自动模拟键盘执行。

6. 完成。

# Payload

payload.dd 文件是使用的 Duckyscript 语法。详细信息请跳转至：<a href="https://docs.hak5.org/hak5-usb-rubber-ducky/duckyscript-tm-quick-reference">https://docs.hak5.org/hak5-usb-rubber-ducky/duckyscript-tm-quick-reference</a>

# 免责声明

本项目固件以及代码均来自互联网；作为键盘模拟程序开发例程，仅供学习使用，请勿用做非法用用途，造成一切后果自行承担！
