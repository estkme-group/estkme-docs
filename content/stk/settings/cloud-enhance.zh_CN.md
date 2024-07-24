+++
linkTitle = "Cloud Enhance"
title = "设置 Cloud Enhance"
weight = 12
+++

{{% notice style="note" title="数据流量使用警告" %}}
Cloud Enhance 需要使用 eSIM 卡通过**蜂窝网络**访问互联网以连接到 Remote LPA 服务器。  
通常，Wi-Fi **不能**用作替代。

网络连接仅在 Cloud Enhance 进程活跃时建立。一旦该过程完成，连接将立刻断开。
{{% /notice %}}

{{% notice style="info" title="关于 Remote LPA 服务器" %}}
Cloud Enhance 依赖**因特网上**的 Remote LPA 服务器。用户可以指定服务器地址以及是否启用该功能。  
Remote LPA 服务器的**源代码**在 **AGPLv3 协议**的条款下免费开放，你可以在 [这里](https://github.com/estkme-group/rlpa-server) 找到源代码。  
你可以按需构建自己的 Remote LPA 服务器。
{{% /notice %}}

## 设置 Cloud Enhance

此菜单包含以下项目：

1. 当前的 Remote LPA 服务器地址，点击以编辑。
2. Cloud Enhance 模式的选项。

> 选项由前缀“\< \>”或“\<\*\>”标识，“\<\*\>”表示当前的选中项。  

Cloud Enhance 模式的可用选项：

- **Enabled**: 启用 Cloud Enhance。
- **Disabled**: 禁用 Cloud Enhance。

## 免责声明

{{% notice style="warning" title="关于网络安全" %}}
在使用 Cloud Enhance 时，eSTK.me 将**通过因特网传输数据**并**与外部 Remote LPA 服务器通信**。  
在使用时，你将面临以下危险：

1. **隐私泄露**
2. **恶意服务器风险**
3. **人为错误的风险**

Cloud Enhance **不能避免**来自运营商的**监控和拦截**。  
**使用此功能即表示你知晓互联网访问费用由你承担并理解可能的服务中断。**
{{% /notice %}}
