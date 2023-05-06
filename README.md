# Bienvenido al repositorio oficial de ReinierTutoriales Compatible con macOS BigSur Monterrey
[![ASUS Z77 P8Z77V LX](https://www.asus.com/media/global/products/wUVREuJSCNu0ys0i/P__setting_xxx_0_90_end_300.png "ASUS Z77 P8Z77V LX")](https://raw.githubusercontent.com/ReinierTutoriales/ASUS-Z77-P8Z77V-LX/main/IMG/1.png "ASUS Z77 P8Z77V LX")
## **Qué contiene este repositorio  👇**
![ASUS Z77 P8Z77V LX](https://raw.githubusercontent.com/ReinierTutoriales/ASUS-Z77-P8Z77V-LX/main/IMG/1.png "ASUS Z77 P8Z77V LX")
Este repositorio contiene el directorio EFI para el combo Intel Intel® Core™ i5-3570K  y MotherBoard ASUS Z77 P8Z77V LX.

![ASUS Z77 P8Z77V LX](https://github.com/ReinierTutoriales/ASUS-Z77-P8Z77V-LX/blob/main/IMG/4.png "ASUS Z77 P8Z77V LX")

## Especificaciones

| Especificaciones     | Detalles                                  |
| ------------------- | -------------------------------------------|
| Motherboard         | ASUS-Z77-P8Z77V-LX                         |
| Procesador          | Intel Core intel i5 3570k                  |
| Memoria RAM         | 16GB/4GB DDR3 1600MHz                      |
| Discp Duro          | SSD Crucial MX500 240GB                    |
| Gráficos Integrados | Intel HD 4000                              |
| Audio               | Realtek ALC255                             |
| Red-Ethernet        | Realtek RTL8111                            |

- **MotherBoard**: ASUS Z77 P8Z77V LX [Compr Aquí](https://www.aliexpress.us/item/2255800711296136.html?aff_fcid=e7b03538d2864373b3a37a112c8ea3ed-1683415274993-08880-_DlDU4WT&tt=CPS_NORMAL&aff_fsk=_DlDU4WT&aff_platform=shareComponent-detail&sk=_DlDU4WT&aff_trace_key=e7b03538d2864373b3a37a112c8ea3ed-1683415274993-08880-_DlDU4WT&terminal_id=5649c23717be4f69b35465125a78381d&afSmartRedirect=y&gatewayAdapt=glo2usa)
- **Procesador**: Intel Core i5-3570K [Compr Aquí](https://www.aliexpress.us/item/2255799827797623.html?aff_fcid=54341684136948a792970115b9bddb36-1683415361500-07163-_DmPfRG7&tt=CPS_NORMAL&aff_fsk=_DmPfRG7&aff_platform=shareComponent-detail&sk=_DmPfRG7&aff_trace_key=54341684136948a792970115b9bddb36-1683415361500-07163-_DmPfRG7&terminal_id=5649c23717be4f69b35465125a78381d&afSmartRedirect=y&gatewayAdapt=glo2usa) 
- **RAM**: [Fury Hyperx - Memoria de escritorio Viper III DDR3 1866MHz (2 x 8 GB) con disipador de calor ](https://s.click.aliexpress.com/e/_DBjbTeR "32GB Corsair Vengeance RGB Pro (2 x 16 GB)DDR4 3600(PC4-28800)memoria optimizada AMD")
- **BT / WIFI**: [Fenvi T919 (BCM94360CD)](https://amzn.to/3w3fkBX "Fenvi T919 (BCM94360CD)")
## Estructura EFI
### Recomendación
- Te recomiendo que uses esto solo como un recurso de referencia.
- Este EFI contiene kexts adicionales en config.plist en lugar de solo las cosas esenciales para la CPU X570 + Zen2. Debe eliminarlos antes de usar esto en su PC.

### Verifique esto antes de usar
En el archivo config.plist , genere códigos de serie nuevos ya que este carece de ellos, pues son personales y cada Mac necesita los de ella propios. Para generar la clave de serie, consulte la Guía OpenCore de Dortania . Cuando genere uno, debe seleccionar MacPro7,1 para un correcto funcionamiento.

### Otro apartado a verificar es
En los nuevos parches de CPU de AMD, ahora tenemos que especificar los recuentos de núcleos de CPU en los algrey - Force cpuid_cores_per_packagenodos. Actualmente, mi configuración de EFI establece para el modelo de CPU de 6 núcleos porque estoy usando Ryzen 5 3600.
[Consulte la descripción del autor para obtener más información.](https://github.com/AMD-OSX/AMD_Vanilla#instructions "Consulte la descripción del autor para obtener más información.")
## OpenCore
**Versión**: 0.8.4

![Opencore 0.8.4](https://github.com/ReinierTutoriales/ASUS-Z77-P8Z77V-LX/blob/main/IMG/6.png?raw=true "Opencore 0.8.4")
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
- AirportItlwm.kext
- AppleALC.kext
- AppleMCEReporterDisabler.kext
- BlueToolFixup.kext
- IntelBluetoothFirmware.kext
- Lilu.kext
- RealtekRTL8111.kext
- RestrictEvents.kext
- SMCProcessor.kext
- SMCSuperIO.kext
- USBInjectAll.kext
- VirtualSMC.kext
- WhateverGreen.kext
## Tools
- OpenShell.efi
- ResetSystem.efi
## Que funciona y que no funciona
### Finciona
- Casi todo, incluida las actualizaciones de Apple (Handoff, iMessage, Airdrop, Facetime, ...)
### Funciona parcialmente
- Tomas de audio de 3,5 mm
- La salida de altavoz en el panel frontal / posterior funciona.
- La entrada de micrófono en el panel frontal / posterior no funciona.
- No he probado la entrada / salida de línea y la salida digital.
- Los problemas habituales de Ryzentosh. Consulte la parte de soporte de CPU de la Guía OpenCore de Dortania
### No funciona
- 
## Referencias
- [OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/ "Dortania's OpenCore Install Guide")
- [forum ReinierTutoriales](https://forum.softgameplus.com/ "forum ReinierTutoriales")
😎
