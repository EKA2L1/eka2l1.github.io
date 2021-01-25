Please utilise the *Table of Contents* by the right to traverse to the section you need.

# Requirements

## For PC version:

### Minimum

- **OS:** Using a **64-bit OS**. For **Windows**, you must have from *Windows 7* and upper
- **Processor:** Any 64-bit CPU from around 2007, starting from **Core 2 Duo E4300**
- **Memory:** 2GB of RAM at minimum
- **Graphics card:** Any OpenGL 3.1 compatible GPU or greater.

### Recommended

- **OS:** Using a **64-bit OS**. For **Windows**, it's recommended to use *Windows 10*
- **Processor:** Any Intel or AMD CPU with 4 cores and upper
- **Memory:** 4GB of RAM or more
- **Graphics card:** Any OpenGL 3.3 compatible GPU or greater.

## For Android version:


### Minimum

- **OS:** Android 5.0 32-bit
- **Processor:** Any ARMv7 CPU or upper. **ARMv6 and down are not supported!**
- **Memory:** 2GB of RAM at minimum
- **Graphics card:** Any OpenGL ES 3.0 compatible GPU or greater

### Recommended
- **OS:** Android 7.0 64-bit (32-bit is experimental)
- **Processor:** An ARMv8 CPU
- **Memory:** 4GB of RAM or more
- **Graphics card:** Any OpenGL ES 3.2 compatible GPU or greater

# Setup
## You need a:
-   ROM (any devices).
-  A repackage of the Z drive (the same device as where the ROM was dumped). See [Dumping section on Wiki](https://github.com/EKA2L1/EKA2L1/wiki/Dumping-the-ROM-and-ROFS) to find out how to dump it.

## Setting up:
- Build or [download](https://12z1.com/download/) EKA2L1.
- You can launch the EKA2L1 directly and interacts with emulator through GUI, or interacts directly through command line.
- Use --help if you want to interact through command lines and need list of commands.
- Install new device through Files/Install device.
  
## Installing new device on EKA2L1
- EKA2L1 has a GUI to install new device. With the GUI, go to Files/Install device.
  ![installdevice](https://camo.githubusercontent.com/08fa49e5578f4045abc98a0cec22bd4bb8cc52480eb3ffab5ed3bee28f7b0e0c/68747470733a2f2f6d656469612e646973636f72646170702e6e65742f6174746163686d656e74732f3536353139363435373433353539343735352f3730303235303631373233383635303937312f756e6b6e6f776e2e706e67)
- Your companion En should guide you through the installation. If a **sudden crash** appears or **device revert installation** because of **falsify reason**, please **contact the developer** for support and fixes if neccessary.
  - If part like determine the Symbian version failed, you should also contact the developers to help improve this automated process.
  
## Change data directory:
- EKA2L1 try to store data within a single folder. By default it's a folder named "data" in the same directory as the executable. You can change the path through GUI in File/Preferences, or change it in **config.yml** with the key **data-storage**.
 - Note that this does not move the data folder. You have to move it yourself.
