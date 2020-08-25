# i5-10500-B460m-Aorus-Pro-Hackintosh-EFI


System:
+ Intel: Core i5-10500
+ Mainboard: Giga B460m Aorus Pro
+ Network: Intel
+ Audio codec: ALC1200A
+ iGPU:UHD 630


Note: - Add kexts: FakePCIID.kext and FakePCIID_Intel_HDMI_Audio.kext fix audio not work

      - Config.plist changes:

        DeviceProperties
        
        PciRoot(0x0)/Pci(0x1F,0x3)
        device-id data 70A10000
        layout-id data 01000000
