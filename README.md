# hackintosh-rog-gx701-efi

基于 [gx531](https://github.com/williambj1/Hackintosh-Asus-ROG-Laptop-Coffee-Lake) 版efi修改而来。

修复gx701的音频、蓝牙、键盘、usb端口等功能，开机会经常性panic重启，应该是pm981硬盘的锅，我没那实力，救不了。

目前来看做开发够用啦。

更新 2023-02-02
---

系统升级到 MacOS 13 Ventura，要求是必须使用 OC 0.8.9 开发版。

1. 更新蓝牙驱动以支持 Ventura
2. 使用开发版 AirportItlwm 驱动以支持 Ventura

更新 2021-08-21
---

移除 Clover 版本，更新 OC 版本到7.2，更新所有 kext，修复触摸板，完善所有设置

1. 经过实验发现触控板无法使用 GPIO 模式，只能使用 POLL 模式
2. 音频偶有爆音问题，按照搜到的资料添加了 `alctsel` 属性，但问题依旧

更新 2021-06-27
---

增加 OpenCore 版配置，WI-FI、蓝牙、音频能用，触控板不能用，没搞好
