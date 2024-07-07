+++
linkTitle = "Using lpac"
title = "Use lpac to download profiles"
weight = 11
+++

{{% notice style="note" title="Notice" %}}
To use with lpac you need a supported PC/SC reader, you can check this by running `lpac driver apdu list`, if it is supported you should see output similar like:

```bash
$ lpac driver apdu list
{"type":"driver","payload":{"env":"DRIVER_IFID","data":[{"env":"0","name":"ACS CCID USB Reader 0"}]}}
```

{{% /notice %}}

lpac is an **open source** LPA software, you can download the release [here](https://github.com/estkme-group/lpac/releases).  
Find out more usage about lpac [here](https://github.com/estkme-group/lpac/blob/main/docs/USAGE.md).

## Use lpac to download your profile

You'll need an [AC code](/manual/activation-code) from your carrier, usually in an email or a physical QR code, some carriers may also require a confirmation code.  
Use the following command to download your profile:  

```bash
# Check that your reader is recognised by lpac
$ lpac driver apdu list
{"type":"driver","payload":{"env":"DRIVER_IFID","data":[{"env":"0","name":"ACS CCID USB Reader 0"}]}}
```

Download your profile with your AC code using `lpac profile download -a "{AC code}"`  
If you have a confirmation code, use `lpac profile download -a "{AC code}" -c "{confirm code}"`  
If successful, you will get `{"type":"lpa","payload":{"code":0,"message":"success","data":null}}`  

```bash
# Download profile using AC code
$ lpac profile download -a LPA:1$SMDP.GSMA.COM$04386-AGYFT-A74Y8-3F815
{"type":"progress","payload":{"code":0,"message":"es10b_get_euicc_challenge_and_info","data":"SMDP.GSMA.COM"}}
{"type":"progress","payload":{"code":0,"message":"es9p_initiate_authentication","data":"SMDP.GSMA.COM"}}
{"type":"progress","payload":{"code":0,"message":"es10b_authenticate_server","data":"SMDP.GSMA.COM"}}
{"type":"progress","payload":{"code":0,"message":"es9p_authenticate_client","data":"SMDP.GSMA.COM"}}
{"type":"progress","payload":{"code":0,"message":"es10b_prepare_download","data":"SMDP.GSMA.COM"}}
{"type":"progress","payload":{"code":0,"message":"es9p_get_bound_profile_package","data":"SMDP.GSMA.COM"}}
{"type":"progress","payload":{"code":0,"message":"es10b_load_bound_profile_package","data":"SMDP.GSMA.COM"}}
{"type":"lpa","payload":{"code":0,"message":"success","data":null}}

```

## Enable your profile

Check your profile list with `lpac profile list`

```bash
$ lpac profile list
{"type":"lpa","payload":{"code":0,"message":"success","data":[{"iccid":"8900000000000000004","isdpAid":"a0000005591010ffffffff8900001000","profileState":"disabled","profileNickname":null,"serviceProviderName":"eSTK.me","profileName":"eSTK.me","iconType":null,"icon":null,"profileClass":"provisioning"}]}}
```

Activate your profile with the iccid you want using `lpac profile enable {iccid}`  
If successful, you will get `{"type":"lpa","payload":{"code":0,"message":"success","data":null}}`  

```bash
$ lpac profile enable "8900000000000000004"
{"type":"lpa","payload":{"code":0,"message":"success","data":null}}
```
