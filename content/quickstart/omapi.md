+++
title = "Android OMAPI"
date =  2023-12-17T00:17:46+08:00
weight = 1
+++

# 如何在安卓设备上使用eSTK
## 你应该准备一部出厂安卓版本在安卓9.0以上的设备和一张eSTK card。
## 本指南使用**EasyEUICC**操作**eSTK**中的Profile，你应当下载并安装**EasyEUICC**，[点击下载](https://gitea.angry.im/PeterCxy/OpenEUICC/releases/download/unpriv-beta02/app-unpriv-release.apk)。

### 第一步：将eSTK插入手机的第一个sim卡槽，打开**EasyEUICC**，若正确识别请进行下一步。
![正确识别eSTK](content/quickstart/omapi/iRN4YbCGpLw6dEG2.jpeg)
#### 若EasyEUICC显示NO EUICC，应逐步排查故障，可以尝试更换eSTK至另一卡槽，可以检查eSTK的ARA-M是否正确配置，也可以更换其它安卓设备尝试。
![eUICC未正确识别](content/quickstart/omapi/105Gn9EKMqnkEPNn.jpeg)
***
### 第二步：如以二维码的形式提供激活码，可使用点击EasyEUICC右下角处 **+** ，直接扫描二维码下载Profile。如以文本形式提供，应解析出SM-DP+服务器地址，激活码(可选)和确认码(可选)后手动下卡。
![开始](content/quickstart/omapi/lOKzQ0rwPEFrJCCF.jpeg)

#### 以LPA:1\$rsp.truphone.com$QR-G-5C-1LS-1W1Z9P7\$45678910为例，其中**rsp.truphone.com**为SM-DP+服务器地址，QR-G-5C-1LS-1W1Z9P7为激活码，45678910为确认码，部分Profile无需激活码和确认码即可下载。
![输入激活码](content/quickstart/omapi/Qf5SLQfIFmXcXLcJ.jpeg)
***
### 第三步：启用Profile，点击Profile右上角三个竖向排列圆点处，选择Enable，等待15-30秒，即可成功启用。期间软件闪退为正常现象。
![启用Profile](content/quickstart/omapi/VrYDjP5R1BiW73Mn.jpeg)
