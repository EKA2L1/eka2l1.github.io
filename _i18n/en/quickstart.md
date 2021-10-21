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

## Files to prepare

### For S60v1 and S60v2 devices (N-Gage, N70, etc...)
- The ROM of the device
- The RPKG file
	- This is a custom container of the Z drive (the same device as where the ROM was dumped). See [Dumping section on Wiki](https://github.com/EKA2L1/EKA2L1/wiki/Dumping-the-ROM-and-ROFS) to find out how to dump it.
	- The file may only be needed with S60v2 devices. The emulator will asks for it during the installation if it detects only ROM alone is not enough.
	
### For S60v3 and upper (5320, 5800, N97, N-Gage 2.0 compatible devices, etc...)

There are two options that you can choose:

- ROM and RPKG of the device (same as S60v1 and S60v2)
- A firmware of the target device. **Make sure** the firmware you got also has a VPL file along with it.

At the moment, for users only interested in N-Gage 2.0, Nokia 5320 device is the most maintained and supported device for this purpose.

## Install a device

- First, build or [download](https://12z1.com/download/) EKA2L1 for the target platform you want to run the emulator on.

### For PC (Windows, MacOS, Linux)

- Launch the emulator with command line option **--help** if you want to interact through command lines and need list of commands.
- To install a new device, please go to *File/Install/Device*, or follow the dialog that ask you to install a device appears on first run of the emulator.

{% include figure image_path="/assets/quickstart/en/device_dialog.png" alt="The device install dialog" caption="The device install dialog" %}

- In this dialog:
	- If you have prepared a ROM (and RPKG if needed), choose the **Device dump** installation method, and click the first *Browse* to select the ROM you have prepared. If the emulator detects that the ROM is not enough alone, a RPKG file browser will appear.
	{% include figure image_path="/assets/quickstart/en/device_dialog_with_rpkg.png" alt="The RPKG field appears with 5320 ROM selected" caption="The RPKG field appears with 5320 ROM selected" %}

	- If you have prepared a firmware, choose the **Firmware (VPL)** installation method. The ROM label will be renamed to VPL, and then you can click *Browse* to choose the VPL that came along with the firmware.
	{% include figure image_path="/assets/quickstart/en/device_dialog_vpl.png" alt="The VPL install dialog" caption="The VPL install dialog" %}

	- **Note**: It's recommended that your path does not contain Unicode or other special characters, the developers are trying to make the emulator more compatible with Unicode paths, but for now the emulator will not work properly with them.

- After you have filled all the paths, press *Install*. If you want to cancel the installation, you can press the *Cancel* button next to *Install*.
	- For **Device dump** installation method, you can wait for the progress bar to be completed and a success dialog to pop up.
	- For **Firmware (VPL)** method, you may need to choose a firmware variant. This usually is related to region of the device and its style (black or red), and should not matter much on the emulator. After that is the same process as **Device dump**.

{% include figure image_path="/assets/quickstart/en/device_dialog_install_success.png" alt="Installation success dialog" caption="Installation success dialog" %}

- If you meets the dialog above, then that means you are done installing a device.

### For Android

- First run of the emulator should show you a dialog that requests you to install a device. Press the *Install* dialog, to quickly get to the **Device manager**.

{% include figure image_path="/assets/quickstart/en/android_device_install_request.jpg" alt="The request install dialog" caption="The request install dialog" %}

- If the dialog does not appear, press the three dots at the top right of your screen, and select **Devices**.

{% include figure image_path="/assets/quickstart/en/android_devices_activity.jpg" alt="Android devices screen" caption="Android devices screen" %}

- In this screen:
	- If you have prepared a ROM (and RPKG if needed), choose the **Device dump** installation method, and press on the *ROM* button to select the ROM you have prepared. If the emulator detects that the ROM is not enough alone, a RPKG file browser will appear.

	- If you have prepared a firmware, choose the **Firmware (VPL)** installation method. The ROM button will be renamed to VPL, and then you can click on the *VPL* button to choose the VPL that came along with the firmware.

	{% include figure image_path="/assets/quickstart/en/android_device_all_choosen.jpg" alt="All file paths are filled" caption="All file paths are filled" %}

- After you have filled all the paths, press *Install*. You can only cancel this operation by exiting the app, and no need further action until a small toast notification tells you that the installation is success or encounters failures.

{% include figure image_path="/assets/quickstart/en/android_new_device_appears.jpg" alt="New device appeared after installation" caption="New device appeared after installation" %}

- **Note**: For Android 11 and upper, the emulator may experiences a huge slow down on device installation, because of the restriction Google applied on files outside of application's private folder (file operations are really slow). We are still coming up with a suitable solution for the emulator.

If you have encountered failure during the installation, please visit the [Discord](https://discord.gg/5Bm5SJ9) server to receive support.

## Install a package (SIS)

### Big note

- Please note that it's very recommended to install a device first and change to the target device you want to install the SIS on, before proceeding this steps.

	- This is crucial for packages like N-Gage 2.0, where it depends on the current active device to extract suitable game configurations file.

### For PC

- Go to *File/Install/Package* and choose the SIS you want to install.


### For Android

- Press on the **big green ``+`` button** on the bottom right of the main (app list) screen and choose the SIS you want to install.

# Managing devices

The emulator allows the users to install multiple devices, and also supports switching between devices. This is neccessary if you want to use applications on different platforms *(S60v1, S60v3)*, without the need for a new instance of emulator with new instance of data folder.

## For PC (Windows, MacOS, Linux)

Go to *File/Settings*, and choose on the *System* tab. The *Devices* section list all of the installed devices.

{% include figure image_path="/assets/quickstart/en/device_manager.png" alt="Device manager section" caption="Device manager section" %}

- Press on the combobox and choose the device you want to run. The changes will be applied immediately.

- You can also rename device for easier management. Press the **Rename** button and enter the new name in the small input dialog.

- Use **Rescan devices** to detect installed devices that does not appear in the combobox.

- Use **Validate current device** for emulator to detect any errors in the device and correct them, in order to make the device runnable on the platform. If the device still does not run, then it means it's either not supported yet or there is another error, you can contact us for more information.

## For Android

The previous screen where you installed devices on is also the device manager screen. Let's take a look at it again.

{% include figure image_path="/assets/quickstart/en/android_new_device_appears.jpg" alt="Device screen" caption="Device screen" %}

- Press on the red circled combo and choose the device you want to run. The changes will be applied immediately.

- You can also rename device for easier management. Press the **Rename** button and enter the new name in the small input dialog.

- Currently there's no rescan or button to validate a device like on PC.

# Change data directory

**Note:** This is only supported on PC. Any faults produced by doing this on Android will not be supported by us.

By default, EKA2L1 stores the data in a **data** folder, sitting at the same location as where the executable *(eka2l1_qt.exe)*. However, if the space is tight or you simply want to move it to more persistent location, you can do that by following these steps:

1. Move the current data folder to your preferred location. **Make sure** the emulator is closed.

2. Change the stored data path of the emulator.

	- With the UI: Go to *File/Settings/General*. You will see the **Data** section appears on the top, press the **Browse** button to select new location, and then the emulator is requested to be restared. After that, your data storage path is completely changed.
	
	{% include figure image_path="/assets/quickstart/en/change_data_folder_pc.png" alt="Data setting section" caption="Data setting" %}

	- With *config.yml* file: This file sits at the same folder as the EKA2L1 executable. Modify the *data-storage* variable in the YAML to the new data path you preferred.
	
# More questions

## Where can I find more guides?

This guide only serves as a quickstart, and will not provide more details on further specific usages. Please visit the [emulator wiki](https://eka2l1.miraheze.org/wiki/Main_Page) for more guides and information.

## I can't get a ROM/RPKG or I can't install, always fail!

It's recommended to visit the [Discord](https://discord.gg/5Bm5SJ9) for support.

You can use a preconfigured pack following the instruction on the [wiki](https://eka2l1.miraheze.org/wiki/How_To_Use_The_Preconfigured_Pack), however it's very large, if you only need to play a specific game/app, install device individually follow the step upper.

## Do you have videos visualise step by step?

We don't have, but there are a lot of videos that have made perfect instructions. It's very recommended to do a search on Youtube for these videos, since we admit that the emulator setup is quite hard.