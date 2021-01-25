Por favor utilize la *Tabla de contenidos* a la derecha para ir al sitio que necesite. 

# Requisitos

## Para la versión de PC:

### Minimos
- **Sistema Operativo:** Debe ser de **64-bit**. Si utilizas **Windows**, es recomendable *Windows 7* o superior
- **Procesador:** Cualquier CPU de 64 bits del 2007 en adelante, empezando por el **Core 2 Duo E4300**
- **Memoria RAM:** 2GB de RAM como mínimo
- **Tarjeta grafíca:** Cualquier GPU compatible con **OpenGL 3.1** o superior

### Recomendados
- **Sistema Operativo:** Debe ser de **64-bit**. Si utilizas **Windows**, es recomendable utilizar *Windows 10* 
- **Procesador:** Cualquier CPU Intel o AMD con 4 nucleos o más
- **Memoria RAM:** 4GB de RAM o más
- **Tarjeta grafíca:** Cualquier GPU compatible con **OpenGL 3.3** o superior

## Para la versión de Android:

### Mínimos
- **Sistema Operativo:** Android 5.0 32-bit
- **Procesador:** Cualquier CPU ARMv7 o superior. **¡ARMv6 y anteriores no están soportados!**
- **Memoria RAM:** 2GB de RAM como mínimo
- **Grafícos:** Cualquier GPU compatible con **OpenGL ES 3.0** o superior

### Recomendados
- **Sistema Operativo:** Android 7.0 64-bit (32-bit sigue en fase experimental)
- **Procesador:** CPU ARMv8 
- **Memoria RAM:** 4GB de RAM o más
- **Grafícos:** Cualquier GPU compatible con **OpenGL ES 3.2** o superior

# Instalación
##  Necesitas:
- ROM (De algún dispositivo Symbian, ejemplos: N-Gage, Nokia N97, Nokia E5)
- Los archivos del drive Z (del mismo dispositivo de donde fue dumpeada la ROM). Ver la [sección](https://github.com/EKA2L1/EKA2L1/wiki/Dumping-the-ROM-and-ROFS) específica
  de la Wiki para aprender como dumpear una ROM tu mismo

## Preparación:
- Descargar [EKA2L1](https://12z1.com/download/)
- Puedes iniciar EAK2L1 directamente e interactuar con el emulador a través de la interfaz grafíca, o puedes hacerlo  directamente a través de comandos
- Usa --help para ver la lista de comandos disponibles (si deseas interactuar con el emulador a través de comandos)
- Instala un nuevo dispositivo a través de Files/Install device
  
## Instalación de un nuevo dispositivo en EKA2L1:
- EKA2L1 tiene una interfaz grafíca que te guía al instalar un nuevo dispositivo. Para encontrarla, vaya a Files/Install device.
  ![installdevice](https://camo.githubusercontent.com/08fa49e5578f4045abc98a0cec22bd4bb8cc52480eb3ffab5ed3bee28f7b0e0c/68747470733a2f2f6d656469612e646973636f72646170702e6e65742f6174746163686d656e74732f3536353139363435373433353539343735352f3730303235303631373233383635303937312f756e6b6e6f776e2e706e67)
- Esta interfaz te guiará a través de la instalación. Si el emulador se **crashea** o la instalación del dispositivo se **revierte** y no logra terminar por **falsify reason**, favor de **contactarse con algun desarrollador** para recibir ayuda y soporte técnico, y en caso de ser necesario, algún parche para reparar el problema
  - Si la instalación falla por que la **determinación de la versión Symbian falló**, también debería contactarse con algún desarrollador y así ayudar a que el emulador mejore

## Cambiar el directorio donde se úbica EKA2L1
- EKA2L1 almacena sus datos en un solo folder. De manera predeterminada, lo hace en una carpeta llamada ''data'' que se encuentra ubicada en la misma carpeta que el ejecutable.
  La dirección de esta carpeta puede ser cambiada a través de la interfaz grafíca en File/Preferences, o de manera manual en el archivo **config.yml**
  - Cabe mencionar que esto **no mueve** de lugar la carpeta, eso tiene que ser hecho de forma manual (cortar y pegar)
