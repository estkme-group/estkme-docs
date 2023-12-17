+++
title = "Virtual EID"
date =  2023-12-17T21:53:42+08:00
weight = 2
+++

## 配置虚拟 EID 的值

配置一个虚拟的 EID 有很多理由，可能为了规避恶意软件的追踪，为了验证某种技术的可行性，或者仅仅是找乐子，此功能可以使 eUICC 管理软件 (LPA) 获取到用户指定的值而并非 eSE 中永久固化的序列号。  
{{% notice style="note" %}}
需要注意的是，当与 Profile 下载服务器(SM-DP+)进行通信时，由于 GSMA PKI 证书系统的存在，虚拟 EID 无法生效，SM-DP+ 总是能获取到 eUICC 的真实 EID 序列号。
{{% /notice %}}

设置 Virtual EID 是一个需要额外注意操作，这意味着：

1. 你可以自由尝试该功能。
2. 该操作的结果是可逆的，或至少有一种恢复先前状态的方法。
3. 特殊的 EID 可能会使一些管理软件异常，确保你可以正常访问 STK 菜单时再进行更改

点击该菜单项后，会自动执行如下步骤

1. 弹出 EID 输入框和提示文字，如果你什么都不输入，意味着关闭该功能
2. 弹出修改成功提示框
3. 向终端设备发起重启 eSTK.me 本身的指令。

{{% notice style="note" %}}
Virtual EID 功能默认仅针对 ISD-R 域有效，如果你需要覆盖 ECASD 域的 EID 读取行为，需要进一步参考 "[ECASD Mode](../ecasd-mode)"
{{% /notice %}}

{{% notice style="warning" %}}
Virtual EID 的设置值无法在 STK 菜单中获取，如果你需要读出，请参考 "[LPA 操作手册](../../../lpa-guide)"
{{% /notice %}}
