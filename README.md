# Bienvenido al repositorio oficial de ReinierTutoriales Compatible con macOS BigSur Monterrey y Ventura
[![ASUS Z77 P8Z77V LX](https://www.asus.com/media/global/products/wUVREuJSCNu0ys0i/P__setting_xxx_0_90_end_300.png "X570 AORUS ELITE")](https://static.gigabyte.com/StaticFile/Image/Global/907eecfe94da125eb443dc223715d8cd/Product/22419/webp/1000 "X570 AORUS ELITE")
## **Qué contiene este repositorio  👇**
Este repositorio contiene el directorio EFI para el combo Ryzen 5 3600 y MotherBoard Gigabyte X570 Aorus Elite.
## Especificación de mi PC
- **MotherBoard**: [Gigabyte X570 Aorus Elite](https://amzn.to/30KCO2k "Gigabyte X570 Aorus Elite")
- **Procesador**: [Ryzen 5 3600](https://amzn.to/3Ag2N0q "Ryzen 5 3600")
- **RAM**: [32GB Corsair Vengeance RGB Pro (2 x 16 GB)DDR4 3600(PC4-28800)memoria optimizada AMD](https://amzn.to/3JPyWiu "32GB Corsair Vengeance RGB Pro (2 x 16 GB)DDR4 3600(PC4-28800)memoria optimizada AMD")
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
## ACPI
- SSDT-PLUG.aml
- SSDT-USBX.aml
- SSDT-XHC.aml 
## Drivers
- HfsPlus.efi
- OpenCanopy.efi
- OpenRuntime.efi
- ResetNvramEntry.efi
- ToggleSipEntry.efi
## Kexts
- AGPMInjector.kext
- AMDRyzenCPUPowerManagement.kext
- AppleALC.kext
- AppleMCEReporterDisabler.kext
- Lilu.kext
- LucyRTL8125Ethernet.kext
- NVMeFix.kext
- RadeonSensor.kext
- RestrictEvents.kext
- SmallTreeIntel82576.kext
- SMCAMDProcessor.kext
- SMCRadeonSensor.kext
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
- Es posible que sea necesario parchear aplicaciones profesionales específicas para procesadores AMD, como aplicaciones de Adobe, Davinci Resolve, etc.
- La virtualización (Apple Hypervisor y las aplicaciones que usan esto como AVD en Android Studio, Parallels) no funciona, pero VirtualBox sí.
### No funciona
- Sidecar
## Referencias
- [OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/ "Dortania's OpenCore Install Guide")
- [forum ReinierTutoriales](https://forum.softgameplus.com/ "forum ReinierTutoriales")
😎
