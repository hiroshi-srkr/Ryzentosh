# OpenCore EFI for AMD Ryzen CPU Hackintosh

## 免責事項

自己責任でご使用ください。万が一、ご使用中のPCに問題が生じた場合、責任は一切負いかねます。
SMBIOS値はご自身で生成してください。config.plistにはダミー値が入っています。


## ハードウェア構成

|　   構成     |                  モデル               　 |
| ------------ | ---------------------------------------- |
| CPU          | AMD Ryzen7 3700X                         |
| MotherBoard  | ASRock B450M Steel Legend                |
| GraphicBoard | SAPPHIRE PULSE Radeon RX VEGA56 8GB HBM2 |
| Memory       | 32GB(2x 16GB)                            |
| Strage       | NVMe SSD 1TB                             |


## 重要な情報

- このEFIはmacOS Sonomaでのみ動作を確認しています。残念ながらSequoiaでは動作しません。
- BuletoothはTPlink社のUB400を想定して設定していますが、残念ながら動作しません。


## 動作する機能

- Sleep
- Ethernet
- iCloud


## 動かない機能（すべてを確認できていません。他にも動かない機能があると思います。）

- Bluetooth
- Wifi
- Sidecar
- VM関連


## Kexts, Kernel Pathces etc

- [AppleALC.kext](https://github.com/acidanthera/applealc/releases)
- [AppleMCEReporterDisabler.kext](https://github.com/acidanthera/bugtracker/files/3703498/AppleMCEReporterDisabler.kext.zip)
- [BlueToolFixup.kext](https://github.com/acidanthera/BrcmPatchRAM/releases)
- [BrcmFirmwareData.kext](https://github.com/acidanthera/BrcmPatchRAM/releases)
- [BrcmPatchRAM3.kext](https://github.com/acidanthera/BrcmPatchRAM/releases)
- [intelBluetoothFirmware.kext](https://github.com/OpenIntelWireless/IntelBluetoothFirmware/releases)
- [IntelBTPatcher.kext](https://github.com/OpenIntelWireless/IntelBluetoothFirmware/releases)
- [Lilu.kext](https://github.com/acidanthera/lilu/releases)
- [NVMeFix.kext]
- [RealtekRTL8111.kext](https://github.com/Mieze/RTL8111_driver_for_OS_X/releases)
- [RestrictEvents](https://github.com/acidanthera/RestrictEvents/releases)
- [SMCRadeonSensors.kext](https://github.com/ChefKissInc/SMCRadeonSensors/releases)
- [USBToolBox.kext](https://github.com/USBToolBox/kext/releases)
- [VirtualSMC](https://github.com/acidanthera/virtualsmc/releases)
- [WhateverGreen](https://github.com/acidanthera/whatevergreen/releases)
- [OpenCore](https://github.com/acidanthera/OpenCorePkg/releases)
- [Kernel Patches](https://github.com/AMD-OSX/AMD_Vanilla)


## BIOSセッティング

|      オプション       |  ステータス  |
| --------------------- | ------------ |
| SATA Mode             | AHCI         |
| Above 4G Decoding     | 有効         |
| EHCI/XHCI Hand-off    | 有効         |
| SVM                   | 有効         |
| CSM                   | 無効         |
| Secure Boot           | 無効         |
| Serial Port           | 無効         |
| Parallel Port         | 無効         |


## ライセンス

このプロジェクトはMITライセンスに基づいてライセンスされています。詳細についてはLICENSE.txtファイルを参照してください。



