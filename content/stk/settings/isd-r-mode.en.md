+++
title = "ISD-R Mode"
date =  2023-12-17T21:54:23+08:00
weight = 6
+++

## Configure the working mode of the ISD-R domain

ISD-R is the main interface for LPA to interact with eUICC, and the management of configuration files (including downloading, switching, deleting, renaming, etc.) and the acquisition of eUICC information are all based on this management domain.

{{% notice style="note" title="Extra Attention Actions" %}}
1. You are free to try the feature.
2. The result of the operation is reversible, or at least there is a way to restore the previous state.
3. Unintended ISD-R mode of operation will cause the LPA application to not be able to manage eUICC, you need to make sure you have access to the STK or have a PCSC card reader.
{{% /notice %}}

The ISD-R Select Menu has a prefix for the < > or <\*> characters, where the <\*> prefix represents the currently active configuration.  

> The ISD-R modes currently available to choose from
1. Shared: The default mode, ISD-R domains can be shared and all access requests are allowed.
2. Exclusive: Exclusive access mode, which requires the current operation to be actively relinquished before accepting other access requests.
3. Disabled: Disabled mode, in which the end device cannot access the ISD-R domain.

{{% notice style="warning" title="Attention" %}}
If you set "[ATR mode](./atr-mode)" to "eUICC" and "Disable ISD-R" at the same time, some terminals may prompt "Smart card is corrupted"
{{% /notice %}}
