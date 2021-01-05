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
        
        PciRoot(0x0)/Pci(0x1b,0x0) => PciRoot(0x0)/Pci(0x1F,0x3)
        device-id data 70A10000
        layout-id data 01000000
      - Off SIP:
      csr-active-config data E7030000
      
Link fix Audio: https://www.reddit.com/r/hackintosh/comments/hmnzj8/catalina_1055_gigbyte_z490gamingx_alc1200a_oc_059/ 
Link fix Pink Screen: https://elitemacx86.com/threads/pink-screen-on-intel-hd-and-uhd-graphics-on-macos-sierra-and-later-on-desktops-clover-opencore.434/?fbclid=IwAR3UWj4SVsJ3ZQFJQol1bdPNqhCieR4a97s0oGonCyIyldYdu3wL8znSPiU
