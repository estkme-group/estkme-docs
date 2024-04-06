+++
title = "Cloud Enhance"
date =  2023-12-17T21:54:11+08:00
weight = 2
+++

## 配置Cloud Enhance

Cloud Enhance依赖位于互联网上的服务器工作，用户需要自行指定服务器地址，以及是否启用该功能。

{{% notice style="note" title="需要网络链接" %}}
使用具体的Cloud Enhance功能需要当前已激活的Profile可通过数据流量访问互联网。通常情况下WiFi无法替代这一要求。
{{% /notice %}}

{{% notice style="warning" title="请注意网络安全" %}}
使用Cloud Enhance提供的功能期间，卡片将会在互联网上传输自身的数据，与外部计算机系统交互。

在此场景下，卡片将面临与一般计算机系统同等的网络安全威胁。

1. 隐私泄露的风险：包括但不限于卡片的唯一识别码、Profile等信息。
2. 恶意服务器的风险：包括但不限于卡片数据被恶意清除、转存、提供给第三方。
3. 其他人为或技术限制引发的风险。

Cloud Enhance无法规避运营商级别的监听与劫持。
{{% /notice %}}

{{% notice style="tip" title="可靠操作" %}}
1. 你可以自由尝试该功能。
2. 该操作的结果是可逆的，或至少有一种恢复先前状态的方法。
{{% /notice %}}

点击该菜单项后，将会弹出：
1. 当前RemoteLPA服务器的地址，点击即可修改。
2. Cloud Enhance工作模式选项。

> 当前可供选择的 Cloud Enhance 模式
1. Enabled : 启用
2. Disabled : 禁用

{{% notice style="info" title="关于服务端" %}}
RemoteLPA服务端是根据AGPL v3协议开源在lpac项目中的，满足公网IPv4与任意一个可访问的TCP端口即可自行架设。
{{% /notice %}}

{{% notice style="tip" title="并非实时链接" %}}
仅仅是启用 Cloud Enhance 功能并不会产生互联网链接，只有在主动使用某项具体的Cloud Enhance功能时才会创建网络链接。一旦功能业务结束，与互联网的链接将立即断开。
{{% /notice %}}
