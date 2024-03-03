+++
title = "Remote LPA"
date =  2023-12-17T21:54:11+08:00
weight = 7
+++

## 配置Remote LPA

Remote LPA依赖位于互联网上的服务器工作，用户需要自行指定服务器地址，以及是否启用该功能。

{{% notice style="tip" title="可靠操作" %}}
1. 你可以自由尝试该功能。
2. 该操作的结果是可逆的，或至少有一种恢复先前状态的方法。
{{% /notice %}}

点击该菜单项后，将会弹出：
1. Remote LPA 服务器的IP地址，仅接受IPv4地址
2. Remote LPA 服务器的端口号
3. Remote LPA 工作模式选项。

> 当前可供选择的 Remote LPA 模式
1. Enabled : 启用Remote LPA功能
2. Disabled : 禁用Remote LPA功能

{{% notice style="info" title="关于服务端" %}}
Remote LPA的服务端是根据AGPL v3协议开源在lpac项目中的，仅需要极低的CPU与内存资源，满足IPv4与任意一个TCP端口即可自行架设。
{{% /notice %}}
