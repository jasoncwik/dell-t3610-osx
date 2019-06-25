# Overview
This is a Clover configuration for running OSX Mojave on the Dell T3610
workstation.

## BIOS settings
* Disable VT-d
* Boot mode AHCI

## Working 

* PCI. Use npci=0x2000. If you change "Number of PCI Busses" in BIOS, you'll need to match this value. (What's Apple's default? Maybe we could set our BIOS)
* (In Progress) USB2. Rename USBE to EH01 and EUSB to EH02. Use USBInjectAll to enable all the ports. Need to fix final port config.
* E5-1620 v2 CPU. Use VoodooTSCSync to prevent hang.
* SSD Trim Support
* Ethernet (IntelMausiEthernet)


## Not Working Yet
* Sleep (hangs on restart)
* USB3 (I hear I just need the standard XHCI driver)

