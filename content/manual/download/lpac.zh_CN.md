+++
linkTitle = "使用 lpac"
title = "使用 lpac 下载 eSIM 卡"
weight = 11
+++

{{% notice style="note" title="注意" %}}
要使用 lpac 你需要一个受支持的 PC/SC 阅读器，你可以运行 `lpac driver apdu list` 来检查这一点，如果支持的话你可以看到类似下面的输出：

```bash
$ lpac driver apdu list
{"type":"driver","payload":{"env":"DRIVER_IFID","data":[{"env":"0","name":"ACS CCID USB Reader 0"}]}}
```

{{% /notice %}}

lpac 是一个**开源**的 LPA 软件你可以在 [这里](https://github.com/estkme-group/lpac/releases) 下载发布的版本。  
在 [这里](https://github.com/estkme-group/lpac/blob/main/docs/USAGE.md) 了解 lpac 的更多用法。

## 使用 lpac 下载你的 eSIM 卡

你需要一个来自你运营商的 [激活码](/manual/activation-code)，通常在一封电子邮件或实体二维码中，一些运营商可能还需要一个确认码。  
使用以下命令来下载你的 eSIM 卡：  

```bash
# 检查你的阅读器是否已被 lpac 识别
$ lpac driver apdu list
{"type":"driver","payload":{"env":"DRIVER_IFID","data":[{"env":"0","name":"ACS CCID USB Reader 0"}]}}
```

使用 `lpac profile download -a "{AC code}"` 通过激活码下载你的 eSIM 卡  
如果还需要确认码，使用 `lpac profile download -a "{AC code}" -c "{confirm code}"`  
如果成功，你将收到 `{"type":"lpa","payload":{"code":0,"message":"success","data":null}}`  

```bash
# 使用激活码下载 eSIM 卡
$ lpac profile download -a LPA:1$SMDP.GSMA.COM$04386-AGYFT-A74Y8-3F815
{"type":"progress","payload":{"code":0,"message":"es10b_get_euicc_challenge_and_info","data":"SMDP.GSMA.COM"}}
{"type":"progress","payload":{"code":0,"message":"es9p_initiate_authentication","data":"SMDP.GSMA.COM"}}
{"type":"progress","payload":{"code":0,"message":"es10b_authenticate_server","data":"SMDP.GSMA.COM"}}
{"type":"progress","payload":{"code":0,"message":"es9p_authenticate_client","data":"SMDP.GSMA.COM"}}
{"type":"progress","payload":{"code":0,"message":"es10b_prepare_download","data":"SMDP.GSMA.COM"}}
{"type":"progress","payload":{"code":0,"message":"es9p_get_bound_profile_package","data":"SMDP.GSMA.COM"}}
{"type":"progress","payload":{"code":0,"message":"es10b_load_bound_profile_package","data":"SMDP.GSMA.COM"}}
{"type":"lpa","payload":{"code":0,"message":"success","data":null}}

```

## 启用你的 eSIM 卡

使用 `lpac profile list` 查看你的 eSIM 卡列表

```bash
$ lpac profile list
{"type":"lpa","payload":{"code":0,"message":"success","data":[{"iccid":"8900000000000000004","isdpAid":"a0000005591010ffffffff8900001000","profileState":"disabled","profileNickname":null,"serviceProviderName":"eSTK.me","profileName":"eSTK.me","iconType":null,"icon":null,"profileClass":"provisioning"}]}}
```

使用 `lpac profile enable {iccid}` 通过对应的 ICCID 激活你想要的 eSIM 卡  
如果成功，你将收到 `{"type":"lpa","payload":{"code":0,"message":"success","data":null}}`  

```bash
$ lpac profile enable "8900000000000000004"
{"type":"lpa","payload":{"code":0,"message":"success","data":null}}
```
