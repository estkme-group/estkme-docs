+++
title = "什么是激活码"
+++

## 什么是激活码

激活码是运营商提供的一串字符串，用于激活你的 eSIM 卡，于 SGP.22 中定义。  
其以 `LPA:1$` 或 `1$` 开头，包含 `SM-DP_ADDRESS` 和 `MATCHING_ID`，中间以 `$` 分隔。  

以下是一些激活码的例子

```text
LPA:1$<SM-DP_ADDRESS>$<MATCHING_ID>
LPA:1$SMDP.GSMA.COM$04386-AGYFT-A74Y8-3F815

1$<SM-DP_ADDRESS>$<MATCHING_ID>
1$SMDP.GSMA.COM$04386-AGYFT-A74Y8-3F815
```

## 如何获得激活码

如果你的运营商提供二维码，则其内容就是你的激活码，你可以使用二维码阅读器读取它。  
一些运营商会随二维码提供 SM-DP 地址和 Matching ID，或直接给你激活码，你可以自行将它们拼接成激活码。  
一些运营商可能还需要**确认码**来下载你的 eSIM 卡，该代码**可能会单独发送**。
