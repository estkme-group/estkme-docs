+++
linkTitle = "使用 EasyEUICC"
title = "通过 EasyEUICC 下载 eSIM 卡"
weight = 13
+++

EasyEUICC 是一个开源的 LPA 软件，你可以在 [这里](https://gitea.angry.im/PeterCxy/OpenEUICC/releases) 下载发布的版本。  
要使用 EasyEUICC，你需要一台带有 **OMAPI 支持**的 **Android 9+** 设备，将你的 eSTK.me 插入**支持 OMAPI 的槽位**中。

## 配置 eSTK.me 以与 EasyEUICC 一起使用

{{% notice style="note" title="注意" %}}
STK 菜单可能**因设备而异**，请先进入你设备上的 eSTK.me 菜单。
{{% /notice %}}

EasyEUICC 通过 **OMAPI** 访问 eSTK.me，你需要将 EasyEUICC 的 ARA-M Hash 置于 eSTK.me 的 [ARA-M 槽](/stk/settings/ara-m) 中。  
eSTK.me **默认带有** EasyEUICC 的 ARA-M Hash，这意味着它可以开箱即用，如果需要，你也可以添加自己的 Hash。  

本例中我们将添加 `2A2FA878BC7C3354C2CF82935A5945A3EDAE4AFA` 到槽位 1。

![imgs](01.png?height=30vh&classes=inline)

![imgs](02.png?height=30vh&classes=inline)

## eSTK.me 无法被 EasyEUICC 检测到？

如果 EasyEUICC 检测不到你的 eSTK.me，检查你的 [ARA-M](/stk/settings/ara-m) Hash 是否正确设置，一些设备需要重启以应用。    
运行兼容性检测来看看你的设备是否支持 **OMAPI**，将 eSTK.me 替换到支持的槽位里。  

如果你的设备与 EasyEUICC 不兼容，改用 lpac 或 Cloud Enhance 以管理你的 eSTK.me。  

- [使用 Cloud Enhance 下载 eSIM 卡](/manual/download/cloud-enhance)
- [通过 lpac 下载 eSIM 卡](/manual/download/lpac)

![imgs](03.png?classes=inline)

## 通过 EasyEUICC 安装 eSIM 卡

打开 EasyEUICC，你在此可以管理 eSTK.me 中的所有 eSIM 卡，如果你有多个 eSE，你可以在右上角切换。  
使用右上角的“New eSIM”，输入你的 [激活码](/manual/activation-code) 或扫描二维码来安装你的 eSIM 卡。  
![imgs](04.png?classes=inline)
