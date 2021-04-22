# fastboot

> Communicate with connected Android devices when in bootloader mode (the one place `adb` doesn't work).
> More information: <https://android.googlesource.com/platform/system/core/+/master/fastboot/#fastboot>.

- Unlock the bootloader:

`fastboot oem unlock`

- Relock the bootloader:

`fastboot oem lock`

- Reboot the device from fastboot mode into fastboot mode again:

`fastboot reboot bootloader`

- Flash a given image (should include boot, vendor, system etc.):

`fastboot flash {{file.zip}}`

- Flash a custom recovery image:

`fastboot flash recovery {{recovery.img}}`

- Flash a custom boot image:

`fastboot flash boot {{boot.img}}`

- Display connected devices:

`fastboot devices`

- Display all information of a device:

`fastboot getvar all`
