+++
title = "ATR Mode"
date =  2023-12-17T21:53:52+08:00
weight = 3
+++

## 配置 eSTK.me 的 ATR 响应

ATR 是智能卡发送给终端的第一段数据，其中包含了从通信方式到数据结构的多种关键信息。

{{% notice style="tip" title="可靠操作" %}}
1. 你可以自由尝试该功能。
2. 该操作的结果是可逆的，或至少有一种恢复先前状态的方法。
{{% /notice %}}

“ATR 选择菜单” 具有 "< >" 或 "<\*>" 字符表示的前缀，其中 "<\*>" 前缀代表的是当前激活的配置。  

> 当前可供选择的 ATR 模式
1. Generic：通用的智能卡ATR通告。
2. eUICC：包含eUICC功能的智能卡。

{{% notice style="warning" title="注意" %}}
如果将 “[ISD-R 模式](./isd-r-mode)” 设置为 “关闭” 的情况下同时通告 eUICC ATR，有可能导致部分终端提示 “智能卡已损坏”
{{% /notice %}}

{{% notice style="info" title="功能限制" %}}
虽然 eSTK.me 具有完全自定义 ATR 的能力，但错误的 ATR 可以轻易的造成软件损坏甚至硬件永久损伤，最终用户仅可在经过安全测试的预设 ATR 数据中进行选择。对于OEM用户，eSTK.me可以提供更丰富的ATR自定义功能并协助测试ATR的可靠性。
{{% /notice %}}
