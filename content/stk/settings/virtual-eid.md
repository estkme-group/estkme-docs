+++
linkTitle = "Virtual EID"
title = "Set Virtual EID"
weight = 13
+++

{{% notice style="note" title="Notice"%}}
**Special EIDs may make some LPAs abnormal**  
When communicating with the SM-DP+ server, the virtual EID **cannot take effect** due to the GSMA PKI certificate, and the server will always receive the **real EID number**.
{{% /notice %}}

## Mock the value of EID in ISD-R

Virtual EID can mock the EID value read by the LPA to the value set by the user.

If Virtual EID is enabled, the EID value **read from the ISD-R** is mocked.

This menu contains the following items:

1. Current Virtual EID value, edit by clicking on it.
2. Options for Virtual EID.

> Options have prefixes represented by "\< \>" or "\<\*\>", where "\<\*\>" indicates the current selection.  

Options available for Virtual EID mode:

- **Enabled**: Enable Virtual EID.
- **Disabled**: Disable Virtual EID.
