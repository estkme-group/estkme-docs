+++
title = "What is AC(activation code)"
+++

## What is AC(activation code)

Activation code is a string provided by the operator to activate your profile, defined in SGP.22.  
It starts with `LPA:1$` or `1$` and contains `SM-DP_ADDRESS` and `MATCHING_ID`, which are separated by `$`.  

Here are some examples of Activation Code:

```text
LPA:1$<SM-DP_ADDRESS>$<MATCHING_ID>
LPA:1$SMDP.GSMA.COM$04386-AGYFT-A74Y8-3F815

1$<SM-DP_ADDRESS>$<MATCHING_ID>
1$SMDP.GSMA.COM$04386-AGYFT-A74Y8-3F815
```

## How to get AC(activation code)

If the carrier provides a QR code, the content of the QR code is your activation code, you can use a QR code scanner to read it.  
Some carriers will provide the SM-DP address and matching ID along with the QR code, or just give you AC, you can assemble them into an AC link yourself.  
Some carriers may also require a **confirmation code** to download your profile, codes **may be sent separately**.
