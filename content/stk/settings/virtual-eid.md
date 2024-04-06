+++
title = "Virtual EID"
date =  2023-12-17T21:53:42+08:00
weight = 3
+++

## 配置虚拟 EID 的值

此功能可以使 eUICC 管理软件 (LPA) 获取到用户指定的值而并非 eSE 中永久固化的序列号。  

{{% notice style="tip" title="可靠操作" %}}
1. 你可以自由尝试该功能。
2. 该操作的结果是可逆的，或至少有一种恢复先前状态的方法。
3. 特殊的 EID 可能会使一些管理软件异常。
{{% /notice %}}

点击该菜单项后，将会弹出：
1. 现有VirtualEID的值，点选将弹出输入框用于更新
2. Virtual EID 工作模式选项

> 当前可供选择的 Virtual EID 模式
1. Enabled：启用 Virtual EID 功能，此时从ISD-R中读取EID将被替换为VirtualEID所设定的值。
2. Disabled：不启用Virtual EID功能。

{{% notice style="note" title="注意" %}}
需要注意的是，当与 Profile 下载服务器 (SM-DP+) 进行通信时，由于 GSMA PKI 证书系统的存在，虚拟 EID 无法生效，SM-DP+ 总是能获取到 eUICC 的真实 EID 序列号。
{{% /notice %}}
