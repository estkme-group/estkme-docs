+++
title = "Process Notifications"
date =  2023-12-17T21:48:31+08:00
weight = 2
+++

## 处理通知

通知是用于同步状态的一种消息，一般用于通知Profile的增加，删除，启用，禁用。

{{% notice style="note" title="Cloud Enhance功能" %}}
该功能需要启用 “[Cloud Enhance](../settings/cloud-enhance)” 功能后方可使用。

本功能需要与互联网交互，用户需自行承担可能存在的风险，详情请阅读 “[Cloud Enhance](./settings/cloud-enhance)” 一节。

当已经有Cloud Enhance事务正在运行时，点击将会展示状态统计页面。
{{% /notice %}}

{{% notice style="tip" title="可靠操作" %}}
1. 你可以自由尝试该功能。
2. 该操作的结果是可逆的，或至少有一种恢复先前状态的方法。
{{% /notice %}}

该功能没有特别的流程，点选后即会后台自动运行。

{{% notice style="tip" title="通知类别" %}}
1. Install: 当尝试安装一个Profile即会产生，有安装成功和安装失败两种不同的通知。
2. Enable: 成功启用一个Profile即会产生，大部分情况下可以直接忽略该通知。
3. Disable: 成功禁用一个Profile即会产生，大部分情况下可以直接忽略该通知。
4. Delete: 成功删除一个Profile即会产生，对于支持多次下载的Profile，成功发送此类通知是非常关键的。
{{% /notice %}}
