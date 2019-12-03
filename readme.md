#Asus X550JK-XO012D, macOS Catalina 10.15.1 with Clover Bootloader 5099

## My PC Specs:
| Specifications  |  Detail |
|---|---|
| Processor |Intel Core i5-4200H 2.80 GHz|
| Memory | 12GB |
| Graphics |<del>NVIDIA GeForce GTX 850M,</del> Intel HD Graphics 4600|  
| Storage |250GB SSD|
| Sound Card |Conexant CX20751/2 |
| Wireless Card |AzureWave CE-123H|

#### BIOS Settings
* VT-D: Disable
* xHCI Mode: Smart Auto
* Secureboot: Disable
* UEFI: Enable
* CSM: Disable

#### What’s Not Working:
* HDMI audio
* <del>Microfone</del>(use apple-alc-id=22 and SSDT-CX20752.dsl and CodecCommander.kext form RehabMan’s bitbucket repo)
* Card Reader

## Kexts

#### Kexts in Library/Extension
* AirportBrcmFixup.kext
* AppleALC.kext
* BrcmBluetoothInjector.kext
* BrcmFirmwareRepo.kext
* BrcmPatchRAM3.kext
* CPUFriend.kext
* Lilu.kext
* NoTouchID.kext
* RealtekRTL8111.kext
* RTCMemoryFixup.kext
* VoodooPS2Controller.kext
* WhateverGreen.kext
      
#### Kexts in Clover/Kexts/Other
* FakePCIID_Intel_HDMI_Audio.kext
* FakePCIID.kext
* SMCBatteryManager.kext
* SMCLightSensor.kext
* SMCProcessor.kext
* SMCSuperIO.kext
* VirtualSMC.kext
      
## Clover      
      
#### Clover Drivers
* ApfsDriverLoader.efi
* AptioMemoryFix.efi
* AudioDxe.efi
* DataHubDxe.efi
* FSInject.efi      
      
#### ACPI files and applied patches 
* SSDT-PNLF.aml
* SSDT-EC.aml
* DSDT
	* “Fix_PARSEOP_ZERO Error
	* “Remove _DSM Methods”
   	* "Fix _WAK Arg0 v2" 
   	* "HPET Fix" 
	* "SMBUS Fix" 
	* "IRQ Fix"  
	* "OS Check Fix" 
	* "Fix Mutex with non-zero SyncLevel"
	* “USB3 _PRW 0x0D (instant wake)”
	* “ASUS N55SL/VivoBook”
* SSDT-1-Cpu0Ist
	* “Remove _PSS placeholders”
* SSDT-6-OptTabl
	* “Cleanup/Fix Errors (SSDT)”


## Usefull Tools and Links
* Hackintool
* Clover Configurator
* [https://github.com/xzhih/one-key-hidpi/]()
* [Lilu and others Guide](https://www.tonymacx86.com/threads/an-idiots-guide-to-lilu-and-its-plug-ins.260063/)
* [USB Port Guide](https://www.tonymacx86.com/threads/the-new-beginners-guide-to-usb-port-configuration.286553/)
* [iMessage Guide](https://www.tonymacx86.com/threads/an-idiots-guide-to-imessage.196827/)