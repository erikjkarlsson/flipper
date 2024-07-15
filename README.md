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

## Usage:

 - Switch to Left Workspace: `<left>` mapped to `S-<left>`
 - Switch to Right Workspace: `<right>` mapped to `S-<right>`
 - Switch Prev Window: `<up>` mapped to `S-<backtab>`
 - Switch Next Window: `<down>` mapped to `S-<tab>`
 - Return: `<select>` mapped to `<return>`
 - Tab: `<back>` mapped to `<tab>`

Where:
   `S-<key>` := `[Super/Win]` + `<key>`

Syntax: `<flipper key>`is mapped to `<keyboard keys>`