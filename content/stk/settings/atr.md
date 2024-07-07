+++
linkTitle = "ATR Mode"
title = "Set ATR Mode"
weight = 5
+++

{{% notice style="warning" title="Warning"%}}
If "[ATR Mode](/stk/settings/atr)" is set to **"eUICC"** and "[ISD-R Mode](/stk/settings/isd-r)" is in **Disable**, some devices may indicate that eSTK.me is corrupted.
{{% /notice %}}

{{% notice style="info" title="Limitation"%}}
Although eSTK.me has the ability to fully customise the ATR, an **incorrect** ATR response can **easily damage equipment**.  
Therefore, users are **only** allowed to select from pre-set ATR data that has undergone safety testing.  
For OEMs, eSTK.me can provide more extensive ATR customisation and assist in testing the reliability of the ATR.  
{{% /notice %}}

## Configure ATR Response for eSTK.me

The ATR is the first block of data sent from the UICC to the device and contains important information such as communication methods, data structures and more.

> Options have prefixes represented by "\< \>" or "\<\*\>", where "\<\*\>" indicates the current selection.  

Options available for ATR mode:

- **Generic**: Announcement as a generic UICC card.
- **eUICC**: Announcement as a UICC with **eUICC related function**.
