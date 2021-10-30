# meson-gxl-s905d-phicomm-n1
## 说明

- 修复负载过高问题
- 修复蓝牙不可用问题

##  使用方法

将项目克隆到本地

`git clone https://github.com/zihelyu/meson-gxl-s905d-phicomm-n1`

进入到meson-gxl-s905d-phicomm-n1目录

`cd meson-gxl-s905d-phicomm-n1`

使用dtc命令将dts编译为dtb

`dtc -I dts -O dtb -o meson-gxl-s905d-phicomm-n1.dtb meson-gxl-s905d-phicomm-n1.dts`

复制dtb到/boot/dtb/amlogic目录

`cp meson-gxl-s905d-phicomm-n1.dtb /boot/dtb/amlogic`

重启服务器

`reboot`

## 其他

本项目在Armbian 20.10测试通过，未测试其他版本，如有问题请提交issues。