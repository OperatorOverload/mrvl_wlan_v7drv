mrvl_wlan_v7drv
===============

Marvell 88W8864 Linux Driver/Firmware Source

The purpose of this fork is to work towards a stable, functional wireless driver that will build against the OpenWRT trunk.

Current State: Will build, not known to be functional

To build this driver with OpenWRT trunk for the WRT1900AC:
1. Clone this repo to a location of your choice.  "git clone https://github.com/OperatorOverload/mrvl_wlan_v7drv.git" will clone into a new folder in the current directory called mrvl_wlan_v7drv
2. Copy the wlan-v7 folder to your openwrt/packages/network folder.
3. Run "make menuconfig"
4. In the menu config, set target system to "Marvell Armada XP/370"
5. Under Kernel Modules -> Wireless Drivers, there is a new entry called "kmod-wlan-v7", select to build this as a Module
6. Make other desired configuration changes, save the configuration, and you're ready to run a "make"
