+++
title = "Cloud Enhance"
date =  2023-12-17T21:54:11+08:00
weight = 2
+++

## Configure Cloud Enhance

Cloud Enrich relies on servers located on the Internet, and users need to specify their own server addresses and whether to enable the feature.

{{% notice style="note" title="Web link required" %}}
To use the specific Cloud Enhance feature, the currently activated Profile can access the internet via data traffic. Often, WiFi can't replace this requirement.
{{% /notice %}}

{{% notice style="warning" title="Be aware of cybersecurity" %}}
During the use of the features provided by Cloud Enhance, the card will transmit its own data over the Internet and interact with external computer systems.

In this scenario, cards are exposed to the same cybersecurity threats as general computer systems.

1. Risk of privacy leakage: including but not limited to the unique identification code of the card, profile and other information.
2. Risks of malicious servers: including but not limited to card data being maliciously cleared, dumped, or provided to third parties.
3. Other Risks Arising from Human or Technological Limitations.

Cloud Enhance does not circumvent carrier-level snooping and hijacking.
{{% /notice %}}

{{% notice style="tip" title="Reliable operation" %}}
1. You are free to try the feature.
2. The result of the operation is reversible, or at least there is a way to restore the previous state.
{{% /notice %}}

When you click on the menu item, it will pop up:
1. The address of the current RemoteLPA server, click to change.
2. Cloud Enhance working mode option

> The Cloud Enhance mode is currently available for selection
1. Enabled
2. Disabled : Disable

{{% notice style="info" title="About the server" %}}
The RemoteLPA server is open-sourced in the LPAC project according to the AGPL v3 protocol, which can be set up by itself to meet the requirements of public IPv4 and any accessible TCP port.
{{% /notice %}}

{{% notice style="tip" title="Not a live link" %}}
Simply enabling the Cloud Enhance feature does not result in an internet link, and only creates a web link when a specific Cloud Enhance feature is actively used. As soon as the functional business ends, the link to the Internet will be immediately disconnected.
{{% /notice %}}
