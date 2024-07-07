+++
linkTitle = "Firmware Update"
title = "Firmware update of eSTK.me"
weight = 5
+++

{{% notice style="note" title="Notice" %}}
To update firmware on eSTK.me you need a standard PC/SC reader.  
After the firmware update, **all configurations will be erased**.
{{% /notice %}}

## Firmware update for eSTK.me on Windows

### 1. Download Firmware Package

The firmware package can be found at <https://www.estk.me/downloads>.  
**Identify your firmware version on the [About](/stk/about) page before you start.**  

### 2. Unzip and Run the update

1. Unzip the downloaded firmware package.
2. Double-click fwupd.exe to initiate the firmware update process.

If you receive the message `boot app done`, your firmware update is complete.

```cmd
estkme-fwupd>fwupd.exe
app erase done
sending sector 1
sector 1 send done
...
...
sector 0 send done
sector 0 write done
boot app done
Press any key to continue...
```

### Troubleshooting:

#### "open smartcard failed"

It means that there is no reader available, try installing a driver or run fwupd.exe as administrator.

#### "SCardListReaders() failed"

If you get `SCardListReaders() failed:` with an error code, check that eSTK.me has good contact with the reader, clean the card and try again.
