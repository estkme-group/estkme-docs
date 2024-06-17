+++
title = "ATR Mode"
date =  2023-12-17T21:53:52+08:00
weight = 5
+++

## Configure the ATR response for eSTK.me

ATR is the first piece of data that a smart card sends to a terminal, and it contains a variety of critical information, from the communication method to the data structure.

{{% notice style="tip" title="Reliable operation" %}}
1. You are free to try the feature.
2. The result of the operation is reversible, or at least there is a way to restore the previous state.
{{% /notice %}}

The ATR Selection Menu has a prefix for the < > or <\*> characters, where the <\*> prefix represents the currently active configuration.  

> The ATR modes currently available to choose from
1. Generic: A generic smart card ATR announcement.
2. eUICC: A smart card that contains the eUICC function.

{{% notice style="warning" title="Attention" %}}
If the eUICC ATR is advertised while "[ISD-R mode](./isd-r-mode)" is set to "Off", it may cause some terminals to prompt "Smart Card is Corrupted"
{{% /notice %}}

{{% notice style="info" title="Feature Limitations" %}}
While eSTK.me has the ability to fully customize ATRs, faulty ATRs can easily cause software damage or even permanent hardware damage, and end users can only choose between preset ATR data that has been tested for safety. For OEM users, eSTK.me can provide more ATR customization capabilities and assist in testing the reliability of ATRs.
{{% /notice %}}
