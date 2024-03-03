+++
title = "ECASD Mode"
date =  2023-12-17T21:54:02+08:00
weight = 5
+++

## 配置 ECASD 管理域的行为

ECASD 是一个特殊的管理域，与 ISD-R 不同，ECASD 保存着 eUICC 最关键的证书与密钥数据，可以理解为是 eUICC 的后端，通常情况下，除了 eSE 的制造方，无需访问 ECASD 域。

{{% notice style="tip" title="配置 ECASD 是一个可靠操作" %}}
1. 你可以自由尝试该功能。
2. 该操作的结果是可逆的，或至少有一种恢复先前状态的方法。
{{% /notice %}}

“ECASD 选择菜单” 具有 "< >" 或 "<\*>" 字符表示的前缀，其中 "<\*>" 前缀代表的是当前激活的配置。

> 当前可供选择的 ECASD 模式
1. Enabled：默认模式，ECASD 可被正常访问。
2. Disabled：禁用模式，在此状态下终端设备无法访问 ECASD 域。
