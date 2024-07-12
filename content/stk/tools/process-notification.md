+++
title = "Process Notification"
weight = 12
+++

{{% notice style="note" title="Disclaimer" %}}
This feature connects to the internet to operate.  
**Use of this feature acknowledges your responsibility for internet access costs and understanding of potential interruptions in service.**  
For more information, visit [Cloud Enhance](/stk/settings/cloud-enhance/#disclaimer)
{{% /notice %}}

{{% notice style="info" title="Config Cloud Enhance First" %}}
You need to config and enable [Cloud Enhance](/stk/settings/cloud-enhance) first to use.  
When Cloud Enhance task is running, status information is displayed on this page.
{{% /notice %}}

{{% notice style="tip" title="Notification Categories" %}}
There are 4 operation types of notifications:

- **Install**: Generated when installing a profile, containing the results of the installation.
- **Enable**: Generated when a profile is activated.
- **Disable**: Generated when a profile is disabled.
- **Delete**: Generated when removing a profile, it is **important** to successfully send this notification.

{{% /notice %}}

## Process notifications on eSTK.me via Cloud Enhance

Process notifications will send notifications in eSE to SM-DP+ Server, after notifications are sent, **notifications will be deleted except for "Delete"**.  
When the process is complete, a pop-up will inform the user of the result and the server will be disconnected.
