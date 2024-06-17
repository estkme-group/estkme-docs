+++
title = "Delete Profile"
date =  2023-12-17T21:23:18+08:00
weight = 4
+++

## Deletes the selected profile

{{% notice style="warning" title="Dangerous Action" %}}
1. The result of the operation is irreversible and one-time in most cases.
2. You need to be very clear about what you're doing and don't blindly accept other people's advice.
3. Deletion within the STK is an "offline deletion", which means that the management server will not be notified immediately when the deletion is made.
{{% /notice %}}

Procedure

1. The delete second confirmation input box and risk warning will pop up
2. The user needs to enter the specified string to confirm the deletion twice
3. A message indicating that the operation was successful or canceled pops up

{{% notice style="info" title="About Takedown Notice" %}}
The STK does not discard the "deletion notice" that should have been sent to the management server, it is actually still stored in the chip and can be sent by the LPA software to the management server again when it is connected to the Internet for "online deletion".
{{% /notice %}}
