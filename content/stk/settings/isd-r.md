+++
linkTitle = "ISD-R Mode"
title = "Set ISD-R Mode"
weight = 16
+++

{{% notice style="warning" title="Warning"%}}
An **unexpected ISD-R mode** will result in the LPA being **unable to manage the eUICC**. You **must** ensure that you have access to the STK or a PC/SC smartcard reader.

If "[ATR Mode](/stk/settings/atr)" is set to **"eUICC"** and "[ISD-R Mode](/stk/settings/isd-r)" is in **Disable**, some devices may indicate that eSTK.me is corrupted.
{{% /notice %}}

## Configure ISD-R domain accessibility

ISD-R is used by the LPA to interact with the eUICC. The management of profiles and the retrieval of eUICC information all use this domain as an entry point.

> Options have prefixes represented by "\< \>" or "\<\*\>", where "\<\*\>" indicates the current selection.  

Options available for ISD-R mode:

- **Shared**: The ISD-R domain can be shared, meaning that all requests to access the ISD-R are allowed.
- **Exclusive**: Access to ISD-R domain is **exclusive**. You must wait for the current operation before you can access it.
- **Disabled**: **Forbid any access** to ISD-R domain.
