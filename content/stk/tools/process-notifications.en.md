+++
title = "Process Notifications"
date =  2023-12-17T21:48:31+08:00
weight = 2
+++

## Handle notifications

A notification is a message used to synchronize the status of a profile, which is generally used to notify the profile of being added, deleted, enabled, or disabled.

{{% notice style="note" title="Cloud Enhance features" %}}
The feature requires "[Cloud Enhance](.. /settings/cloud-enhance)" function.

This feature requires interaction with the Internet and the user is at the user's own risk, please read the section "[Cloud Enhance](./settings/cloud-enhance)" for details.

When a Cloud Enhance transaction is already running, clicking on it will display the status statistics page.
{{% /notice %}}

{{% notice style="tip" title="Reliable operation" %}}
1. You are free to try the feature.
2. The result of the operation is reversible, or at least there is a way to restore the previous state.
{{% /notice %}}

There is no special process for this function, and it will run automatically in the background after clicking.

{{% notice style="tip" title="Notification Category" %}}
1. Install: When you try to install a profile, you will be notified that the installation is successful and the installation is unsuccessful.
2. Enable: Generated when a profile is successfully enabled, in most cases, the notification can be ignored directly.
3. Disable: Successfully disabling a profile will occur, and in most cases you can ignore the notification.
4. Delete: Successful deletion of a profile is generated, and it is critical to send such a notification successfully for profiles that support multiple downloads.
{{% /notice %}}
