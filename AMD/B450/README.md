# AMD B450

## Computer Specification
<table>
  <thead>
    <tr>
      <th align="left">Component</th>
      <th align="left">Model</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="left">CPU</td>
      <td align="left">AMD Ryzen 5 5600X @ 3.7GHz</td>
    </tr>
    <tr>
      <td align="left">Motherboard</td>
      <td align="left">MSI B450M-A PRO MAX</td>
    </tr>
    <tr>
      <td align="left">RAM</td>
      <td align="left">32GB (2 x 16GB) HyperX Fury DDR4 @ 2666MHz</td>
    </tr>
    <tr>
      <td align="left">GPU</td>
      <td align="left">AMD XFX 210 RX 6600 XT</td>
    </tr>
    <tr>
      <td align="left">Audio Chipset</td>
      <td align="left">Realtek ALC897 Codec</td>
    </tr>
    <tr>
      <td align="left">Ethernet</td>
      <td align="left">Realtek RTL8111</td>
    </tr>
    <tr>
      <td align="left">OS Disk</td>
      <td align="left">Kingston A400 SSD 120GB</td>
    </tr>
  </tbody>
</table>

## Tested Versions
<table>
  <thead>
    <tr>
      <th align="left">System</th>
      <th align="left">Version</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="left">macOS</td>
      <td align="left">13.3.1</td>
    </tr>
    <tr>
      <td align="left">OpenCore</td>
      <td align="left">0.9.2</td>
    </tr>
  </tbody>
</table>

## Boot Args
- Debug
  -  > -v keepsyms=1 debug=0x100 alcid=100 agdpmod=pikera
- Release
  -  > alcid=100 agdpmod=pikera

## BIOS Config
#### Disable:
- fast boot
- secury boot
- serial COM
- resize bar
#### Enable:
- 4G decoding
- SATA operations to AHCI
- XCHCI USB

## Working
#### Tested:
- [x] iCoud
- [x] Ethernet
- [x] Audio
- [ ] CPU Name
#### Untested:
- [ ] Bluetooth
- [ ] Wifi

## Kexts
- <a href="https://github.com/dortania/Getting-Started-With-ACPI/blob/master/extra-files/compiled/SSDT-EC-USBX-DESKTOP.aml">SSDT EC USBX DESKTOP</a>

## Drivers
- <a href="https://github.com/luchina-gabriel/BASE-EFI-AMD-RYZEN-THREADRIPPER/blob/main/EFI-Debug/OC/Drivers/AudioDxe.efi">Audio Dxe</a>
- <a href="https://github.com/luchina-gabriel/BASE-EFI-AMD-RYZEN-THREADRIPPER/blob/main/EFI-Debug/OC/Drivers/HfsPlus.efi">HfsPlus</a>
- <a href="https://github.com/acidanthera/OpenCorePkg/releases">Open Canopy</a>
- <a href="https://github.com/luchina-gabriel/BASE-EFI-AMD-RYZEN-THREADRIPPER/blob/main/EFI-Debug/OC/Drivers/OpenRuntime.efi">Open Runtime</a>
- <a href="https://github.com/luchina-gabriel/BASE-EFI-AMD-RYZEN-THREADRIPPER/blob/main/EFI-Debug/OC/Drivers/ResetNvramEntry.efi">Reset NVRAM Entry</a>

## Kexts
- <a href="https://github.com/acidanthera/Lilu/releases">Lilu</a>
- <a href="https://github.com/acidanthera/VirtualSMC/releases">Virtual SMC</a>
- <a href="https://github.com/trulyspinach/SMCAMDProcessor/releases">AMD Ryzen CPU Power Management</a>
- <a href="https://github.com/trulyspinach/SMCAMDProcessor/releases">SMC AMD Processor</a>
- <a href="https://github.com/acidanthera/AppleALC/releases">Apple ALC</a>
- <a href="https://dortania.github.io/OpenCore-Install-Guide/ktext.html#extras">Apple MCE Reporter Disabler</a>
- <a href="https://github.com/Mieze/RTL8111_driver_for_OS_X/releases">Realtek RTL 8111</a>
- <a href="https://github.com/acidanthera/RestrictEvents/releases">Restrict Events</a>
- <a href="https://github.com/corpnewt/USBMap">USB Map</a>
- <a href="https://github.com/corpnewt/USBMap">USB Map Legacy</a>
- <a href="https://github.com/acidanthera/WhateverGreen/releases">Whatever Green</a>

### Based on
<a href="https://github.com/luchina-gabriel/BASE-EFI-AMD-RYZEN-THREADRIPPER">Gabriel Luchina AMD EFI</a>