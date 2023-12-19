+++
title = "ISD-R Mode"
date =  2023-12-17T21:54:23+08:00
weight = 4
+++

## 配置 ISD-R 域的工作模式

ISD-R 是 LPA 与 eUICC 进行交互的主要接口，配置文件的管理（包括下载，切换，删除，重命名等）、eUICC 信息的获取，均以该管理域为入口。
修改 ISD-R 的工作模式需要额外注意操作，这意味着：

1. 你可以自由尝试该功能。
2. 该操作的结果是可逆的，或至少有一种恢复先前状态的方法。
3. 非预期的 ISD-R 工作模式会导致 LPA 应用无法管理 eUICC，需要确保你可以正常访问 STK 或拥有 PCSC 读卡器。

“ISD-R 选择菜单” 具有 "< >" 或 "<\*>" 字符表示的前缀，其中 "<\*>" 前缀代表的是当前激活的配置。  
>当前可供选择的 ISD-R 模式

1. Shared：默认模式，ISD-R 域可被共享访问，所有访问请求均被允许。
2. Exclusive：独占访问模式，必须等待当前操作主动让出才可接受其他访问请求。
3. Disabled：禁用模式，在此状态下终端设备无法访问 ISD-R 域。