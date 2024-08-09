+++
linkTitle = "Using EasyEUICC"
title = "Use EasyEUICC to download profiles"
weight = 13
+++

EasyEUICC is an open source LPA software, you can download the release [here](https://gitea.angry.im/PeterCxy/OpenEUICC/releases).  
To use EasyEUICC you need an **Android 9+** device with **OMAPI support**, insert your eSTK.me into the **OMAPI supported slot**.

## Configure eSTK.me for use with EasyEUICC

{{% notice style="note" title="Notice" %}}
STK menu **may vary by device**, please enter the eSTK.me menu on your device fisrt.
{{% /notice %}}

EasyEUICC access eSTK.me via **OMAPI**, you need to put EasyEUICC's ARA-M hash to eSTK.me's [ARA-M slot](/stk/settings/ara-m).  
eSTK.me comes with EasyEUICC's ARA-M hash **by default**, this means it works right out of the box, you can add your own if you wish.  

In this case we will add `2A2FA878BC7C3354C2CF82935A5945A3EDAE4AFA` to slot 1.  
![imgs](01.png?height=30vh&classes=inline)![imgs](02.png?height=30vh&classes=inline)  

## eSTK.me not detected by EasyEUICC?

If EasyEUICC did not detect your eSTK.me, check that your [ARA-M](/stk/settings/ara-m) hash is set correctly, some devices may need a reboot to apply it.  
Run a compatibility check to see if your device supports **OMAPI**, swap eSTK.me to a **supported slot**.  

If your device is not compatible with EasyEUICC, use lpac or Cloud Enhance to manage your eSTK.me instead.  

- [Use Cloud Enhance to download profiles](/manual/download/cloud-enhance)
- [Use lpac to download profiles](/manual/download/lpac)

![imgs](03.png?classes=inline)  

## Install profiles with EasyEUICC

Open EasyEUICC, you can manage all your profiles in eSTK.me, if you have multiple eSE, you can switch on the top right corner.  
Use the "New eSIM" button in the bottom right corner, fill in your [AC code](/manual/activation-code) or scan the QR code to install your profile.  
![imgs](04.png?classes=inline)
