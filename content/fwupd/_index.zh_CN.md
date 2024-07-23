+++
linkTitle = "固件升级"
title = "升级 eSTK.me 的固件"
weight = 5
+++

{{% notice style="note" title="注意" %}}
你需要一个标准 PC/SC 阅读器来升级 eSTK.me 的固件。  
固件升级后，**所有设置都将被擦除**。
{{% /notice %}}

## 在 Windows 上升级 eSTK.me 的固件

### 1. 下载固件包

固件包可在 <https://www.estk.me/downloads> 找到。  
**开始之前，在 [About](/stk/about) 页面确认你的固件版本。**  

### 2. 解压并执行升级

1. 解压下载的固件包。
2. 双击 fwupd.exe 以开始固件升级过程。

如果收到信息 `boot app done`，说明固件已完成升级。

```cmd
estkme-fwupd>fwupd.exe
app erase done
sending sector 1
sector 1 send done
...
...
sector 0 send done
sector 0 write done
boot app done
Press any key to continue...
```

### 疑难解答

#### "open smartcard failed"

这说明没有可用的阅读器，尝试安装驱动或以管理员身份运行 fwupd.exe。

#### "SCardListReaders() failed"

如果收到带有错误码的 `SCardListReaders() failed:` 提示，检查 eSTK.me 与阅读器的接触是否良好，清洁卡片，然后重试。
