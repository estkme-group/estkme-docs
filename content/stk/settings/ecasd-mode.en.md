+++
title = "ECASD Mode"
date =  2023-12-17T21:54:02+08:00
weight = 7
+++

## Configure the behavior of the ECASD management domain

ECASD is a special management domain, unlike ISD-R, ECASD holds the most critical certificate and key data of eUICC, which can be understood as the backend of eUICC, and usually, except for the manufacturer of eSE, there is no need to access the ECASD domain.

{{% notice style="tip" title="Configuring ECASD is a reliable operation" %}}
1. You are free to try the feature.
2. The result of the operation is reversible, or at least there is a way to restore the previous state.
{{% /notice %}}

The ECASD Selection Menu has a prefix for the < > or <\*> characters, where the <\*> prefix represents the currently active configuration.

> The ECASD modes currently available to choose from
1. Enabled: ECASD can be accessed normally by default.
2. Disabled: Disabled mode, in which the end device cannot access the ECASD domain.
