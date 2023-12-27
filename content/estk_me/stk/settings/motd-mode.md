+++
title = "MOTD Mode"
date =  2023-12-17T21:54:11+08:00
weight = 7
+++

## 开启或者关闭欢迎语

{{% notice style="note" title="注意" %}}
[Hint Mode](./hint-mode) 于固件版本 1.2.3.1 中加入，于固件版本 1.2.5.1 中更名为 MOTD Mode。  
eSTK.me 固件版本信息在固件版本 1.2.6 中加入。
{{% /notice %}}

MOTD 用于在 eSTK.me 插入设备后提示用户 eSTK.me 已被识别，用户将在重启设备或 eSTK.me 插入时看到 `HelloWorld!` 提示与当前 eSTK.me 的固件版本号。  
配置 MOTD 是一个可靠操作，这意味着：

1. 你可以自由尝试该功能。
2. 该操作的结果是可逆的，或至少有一种恢复先前状态的方法。

>当前可供选择的 MOTD 模式

1. Enabled : 启用欢迎语功能
2. Disabled : 禁用欢迎语功能
