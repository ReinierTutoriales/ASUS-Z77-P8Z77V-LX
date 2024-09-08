# Bienvenido al repositorio oficial de ReinierTutoriales compatible con macOS 11 Big Sur, macOS 12 Monterrey, macOS 13 Ventura, macOS 14 Sonoma y macOS 15 Sequoia.

![macOS Sonoma](IMG/1.png)


[![Static Badge](https://img.shields.io/badge/ISOS-macOS-blue)](https://www.reiniertutoriales.com/forums/isos-macos.10/)
[![Static Badge](https://img.shields.io/badge/OpenCore-1.0.2-green)](https://github.com/dortania/build-repo/releases/download/OpenCorePkg-fa4112e/OpenCore-1.0.2-RELEASE.zip)
[![GitHub issues](https://img.shields.io/github/issues/ReinierTutoriales/ASUS-Z77-P8Z77V-LX)](https://github.com/ReinierTutoriales/ASUS-Z77-P8Z77V-LX/issues)

[![](https://img.shields.io/badge/YouTube-informational?style=for-the-badge&logo=telegram&logoColor=white&color=FF0000)](https://youtube.com/c/ReinierTutoriales)
[![](https://img.shields.io/badge/PayPal-informational?style=for-the-badge&logo=paypal&logoColor=white&color=003087)](https://www.paypal.com/paypalme/ReinierTutoriales)
[![](https://img.shields.io/badge/-Telegram-informational?style=for-the-badge&logo=telegram&logoColor=white&color=0088cc)](https://t.me/ReinierTutoriales)
[![](https://img.shields.io/badge/-Twitter-informational?style=for-the-badge&logo=twitter&logoColor=white&color=00aced)](https://twitter.com/ReinierTutorial)
[![](https://img.shields.io/badge/-Facebook-informational?style=for-the-badge&logo=facebook&logoColor=white&color=3b5998)](https://www.facebook.com/ReinierTutoriales)
[![](https://img.shields.io/badge/-Instagram-informational?style=for-the-badge&logo=instagram&logoColor=white&color=C13584)](https://www.instagram.com/reiniertutoriales/)
[![](https://img.shields.io/badge/-Discord-informational?style=for-the-badge&logo=discord&logoColor=white&color=7289da)](https://discord.gg/pQcCDBMn)

</p>


# Apóyame con una donación 
Mediante [👉PayPal💵](https://www.paypal.com/paypalme/ReinierTutoriales?country.x=US&locale.x=es_XC)



# **Qué contiene este repositorio  👇**
Este repositorio contiene el directorio EFI para el combo Intel Intel® Core™ i5-3570K  y MotherBoard ASUS Z77 P8Z77V LX.


## Especificaciones

| Especificaciones     | Detalles                                  |
| ------------------- | -------------------------------------------|
| Motherboard         |  `ASUS-Z77-P8Z77V-LX`                      |
| Procesador          | Intel Core intel `i5 3570k`                |
| Memoria RAM         | `16GB`/`4GB` DDR3 1600MHz                  |
| Disco Duro          | SSD  `Crucial MX500` `240GB`               |
| Gráficos Integrados | Intel  `HD 4000`                           |
| Audio               | Realtek `ALC255`                           |
| Red-Ethernet        | Realtek `RTL8111`                          |

- **MotherBoard**: ASUS Z77 P8Z77V LX [👉Compr Aquí💵](https://s.click.aliexpress.com/e/_DEav2bR)
- **Procesador**: Intel Core i5-3570K [👉Compr Aquí💵](https://s.click.aliexpress.com/e/_DezOy29) 
- **RAM**: 2x8GB Fury Hyperx Viper III DDR3 1866MHz [👉Compr Aquí💵](https://s.click.aliexpress.com/e/_Ddspq81)
- **BT / WIFI**: Fenvi T919 (BCM94360CD) [👉Compr Aquí💵](https://amzn.to/3w3fkBX)

# Recomendación
- Te recomiendo que uses esto solo como un recurso de referencia.
- Este EFI contiene kexts adicionales en config.plist en lugar de solo las cosas esenciales para la ASUS Z77 P8Z77V LX. Debe eliminarlos antes de usar esto en su PC.

# Verifique esto antes de usar
En el archivo config.plist , genere códigos de serie nuevos ya que este carece de ellos, pues son personales y cada Mac necesita los de ella propios. Para generar la clave de serie, consulte la Guía OpenCore de Dortania . Cuando genere uno, debe seleccionar MacPro7,1 para un correcto funcionamiento.


# OpenCore
**Versión**: 1.0.2

# Estructura EFI
## ACPI
- SSDT-EC-DESKTOP.aml
- SSDT-IMEI.aml
- SSDT-PM.aml
## Drivers
- HfsPlus.efi
- OpenCanopy.efi
- OpenRuntime.efi
- ResetNvramEntry.efi
- ToggleSipEntry.efi
## Kexts
- AMFIPass.kext
- AppleALC.kext
- AppleIntelCPUPowerManagement.kext
- AppleIntelCPUPowerManagementClient.kext
- CryptexFixup.kext
- Lilu.kext
- RealtekRTL8111.kext
- RestrictEvents.kext
- SMCProcessor.kext
- SMCSuperIO.kext
- USBToolBox.kext
- UTBMap.kext
- VirtualSMC.kext
- WhateverGreen.kext

## Tools
- OpenShell.efi
- ResetSystem.efi

# Que Finciona
- Casi todo, incluida las actualizaciones de Apple (Handoff, iMessage, Airdrop, Facetime)
 
# Referencias
- [OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/ "Dortania's OpenCore Install Guide")
- [Blog ReinierTutoriales](https://www.reiniertutoriales.com)
😎
