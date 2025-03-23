# 🔧 AMD B450 Configuration

## 🖥️ Hardware Specifications

| Component      | Model                            |
|----------------|----------------------------------|
| CPU            | AMD Ryzen 5 5600X @ 3.7GHz       |
| Motherboard    | MSI B450M-A PRO MAX              |
| RAM            | 32GB (2 x 16GB) HyperX Fury DDR4 @ 2666MHz |
| GPU            | AMD XFX 210 RX 6600 XT           |
| Audio Chipset  | Realtek ALC897 Codec             |
| Ethernet       | Realtek RTL8111                  |
| OS Disk        | Kingston A400 SSD 120GB          |

## ✅ Tested Versions

| Software       | Version |
|----------------|---------|
| macOS          | 13.3.1  |
| OpenCore       | 0.9.2   |

---

## 🚦 BIOS Configuration

### 🔴 Disable:
- Fast Boot
- Secure Boot
- Serial COM
- Resize BAR

### 🟢 Enable:
- 4G Decoding
- SATA Operation (AHCI)
- XHCI USB

---

## 📌 Boot Arguments

### 🛠️ Debug
```
-v keepsyms=1 debug=0x100 alcid=100 agdpmod=pikera
```

### 🚀 Release
```
alcid=100 agdpmod=pikera
```

---

## 🔎 Component Status

### ✅ Working
- iCloud
- Ethernet
- Audio

### ⚠️ Partially Working
- CPU Name

### 🚧 Untested
- Bluetooth
- Wi-Fi

---

## 🔌 Kexts and Drivers

### 📂 Drivers
- [AudioDxe.efi](https://github.com/luchina-gabriel/BASE-EFI-AMD-RYZEN-THREADRIPPER)
- [HfsPlus.efi](https://github.com/luchina-gabriel/BASE-EFI-AMD-RYZEN-THREADRIPPER)
- [OpenCanopy](https://github.com/acidanthera/OpenCorePkg/releases)
- [OpenRuntime.efi](https://github.com/luchina-gabriel/BASE-EFI-AMD-RYZEN-THREADRIPPER)
- [ResetNvramEntry.efi](https://github.com/luchina-gabriel/BASE-EFI-AMD-RYZEN-THREADRIPPER)

### 📂 Kexts
- [Lilu](https://github.com/acidanthera/Lilu/releases)
- [VirtualSMC](https://github.com/acidanthera/VirtualSMC/releases)
- [AMD Ryzen CPU Power Management](https://github.com/trulyspinach/SMCAMDProcessor/releases)
- [SMC AMD Processor](https://github.com/trulyspinach/SMCAMDProcessor/releases)
- [AppleALC](https://github.com/acidanthera/AppleALC/releases)
- [Apple MCE Reporter Disabler](https://dortania.github.io/OpenCore-Install-Guide/ktext.html#extras)
- [Realtek RTL8111](https://github.com/Mieze/RTL8111_driver_for_OS_X/releases)
- [RestrictEvents](https://github.com/acidanthera/RestrictEvents/releases)
- [USBMap](https://github.com/corpnewt/USBMap)
- [USBMap Legacy](https://github.com/corpnewt/USBMap)
- [WhateverGreen](https://github.com/acidanthera/WhateverGreen/releases)

---

## 📚 Based on

- [Gabriel Luchina AMD EFI](https://github.com/luchina-gabriel/BASE-EFI-AMD-RYZEN-THREADRIPPER-PUBLIC)

---

