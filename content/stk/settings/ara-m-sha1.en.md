+++
title = "ARA-M SHA-1"
date =  2023-12-17T21:48:31+08:00
weight = 1
+++

## GRANT APP ACCESS

ARA-M is a special property of smart cards that is used to control which applications can access the smart card interface on modern operating systems. It is now widely used on the Android operating system that supports OMAPI.  
The smart card uses ARA-M to notify the operating system through the value of the developer's certificate SHA-1 or SHA-256 that the app is from which developer the app can access it.

{{% notice style="note" title="Extra Attention Actions" %}}
1. You are free to try the feature.
2. The result of the operation is reversible, or at least there is a way to restore the previous state.
3. Incorrect values for ARA-M SHA-1 will cause LPA applications to not be able to manage eUICC, you need to make sure you have access to the STK or have a PCSC reader.
{{% /notice %}}

When you click on this menu item, 5 ARA-M values that have been stored in the card will be listed, and if they have never been set, all zeros will be displayed.

Click any value to enter the edit mode, which has the following two operations:

1. Enter the expected SHA-1 value, which will be saved in the card.
2. If no information is entered and submitted, the previously selected value will be zeroed.

{{% notice style="note" title="note" %}}
If you mistakenly change the ARA-M SHA-1 value and you can't access the STK menu properly, you need to refer to the "Firmware Upgrade" section to restore the settings to the factory state. 
{{% /notice %}}

{{% notice style="tip" title="tip" %}}
eSTK.me Up to 5 different ARA-Ms are currently supported. This means that you can authorize apps from up to 5 different developers to manage your cards.
{{% /notice %}}

{{% expand title="Before 1.2.3 firmware"%}}
{{% /expand %}}
