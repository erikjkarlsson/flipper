# How to build "Navigator" (Hack to the HID Controller)

## New Files:

 1. `./apps/hid_usb2/views/hid_navigator.c`
 2. `./apps/hid_usb2/views/hid_navigator.h`

## Building

 1. Link apps to `Xtreme-Firmware/applications_user`: 

  * Remove default user app folder: `$ rm -r ./Xtreme-Firmware/applications_user`
  * Link custom folder: `$ ln -sr ./apps ./Xtreme-Firmware/applications_user`

 2. Build using the *flipper build tool*:

  * `$ cd ./Xtreme-Firmware/`

  * Build Bluetooth controller: `./fbt build APPSRC=hid_ble2`
  * Test Bluetooth controller: `./fbt launch APPSRC=hid_ble2`  

  * Build USB controller: `./fbt build APPSRC=hid_usb2`
  * Test USB controller: `./fbt launch APPSRC=hid_usb2`  

