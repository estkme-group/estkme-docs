+++
linkTitle = "ARA-M SHA-1"
title = "Config ARA-M Slot"
weight = 11
+++

{{% notice style="note" title="Notice" %}}
An incorrect ARA-M will cause the LPA application unable to manage the eUICC. You need to ensure that you can access the STK or have a PC/SC reader.
{{% /notice %}}

ARA-M, as a special application of smartcards, is used to control which applications can access the smartcard. It is widely used on Android devices that support OMAPI.  
UICC uses the SHA-1 or SHA-256 values of the application certificate signatures in ARA-M to inform the operating system which applications can access the card.

## Grant access to APP using ARA-M

{{% notice style="tip" %}}
If no characters are entered, the value of the ARA-M in the slot is set to zero.
{{% /notice %}}

There are 5 ARA-M slots in eSTK.me, select any slot to enter edit mode, enter the SHA-1 of the APP you want to store in the slot.
