+++
title = "Virtual EID"
date =  2023-12-17T21:53:42+08:00
weight = 3
+++

## Configure the value of the virtual EID

This feature allows the eUICC Management Software (LPA) to obtain a user-specified value instead of the permanently solidified serial number in the eSE.  

{{% notice style="tip" title="Reliable operation" %}}
1. You are free to try the feature.
2. The result of the operation is reversible, or at least there is a way to restore the previous state.
3. Special EIDs may make some management software abnormal.
{{% /notice %}}

When you click on the menu item, it will pop up:
1. The value of the existing VirtualEID, click on the input box that will pop up for updating
2. Virtual EID working mode option

> The Virtual EID modes currently available to choose from
1. Enabled: Enable the Virtual EID function, at which point reading the EID from ISD-R will be replaced with the value set by VirtualEID.
2. Disabled: The Virtual EID feature is disabled.

{{% notice style="note" title="note" %}}
It is important to note that when communicating with the Profile Download Server (SM-DP+), the virtual EID cannot be activated due to the GSMA PKI certificate system, and SM-DP+ will always be able to obtain the real EID serial number of the eUICC.
{{% /notice %}}
