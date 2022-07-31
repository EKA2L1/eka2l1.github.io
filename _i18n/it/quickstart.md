Per favore, utilizza la *Tabella dei Contenuti* a destra per navigare tra le sezioni che ti servono.

# Requisiti

## Per la versione PC:

### Minimo

- **Sistema Operativo:** Usare un **OS 64-bit**. Per **Windows**, devi avere *Windows 7* o superiore
- **Processore:** Qualsiasi CPU 64-bit a partire dal 2007 circa, per esempio il **Core 2 Duo E4300**
- **Memoria RAM:** Minimo 2GB di RAM
- **Scheda grafica:** Qualsiasi GPU compatibile OpenGL 3.1 o superiore.

### Consigliato

- **Sistema Operativo:** Usare un **OS 64-bit**. Per **Windows**, è consigliato l'uso di *Windows 10*
- **Processore:** Qualsiasi CPU AMD o Intel con 4 o più core
- **Memoria RAM:** 4GB di RAM o più
- **Scheda grafica:** Qualsiasi GPU compatibile OpenGL 3.3 o superiore.

## Per la versione Android:


### Minimo

- **Sistema Operativo:** Android 5.0 32-bit
- **Processore:** Qualsiasi CPU ARMv7 o superiore. **ARMv6 e precedenti non sono supportati!**
- **Memoria RAM:** Minimo 2GB di RAM
- **Scheda grafica:** Qualsiasi GPU compatibile OpenGL ES 3.0 o superiore.

### Consigliato
- **Sistema Operativo:** Android 7.0 64-bit (32-bit è sperimentale)
- **Processore:** Una CPU ARMv8
- **Memoria RAM:** 4GB di RAM o più
- **Scheda grafica:** Qualsiasi GPU compatibile OpenGL ES 3.2 o superiore.

# Installazione

## File da preparare

### Per dispositivi S60v1 e S60v2 (N-Gage, N70, ecc...)
- La ROM del dispositivo
- Il file RPKG
	- Questo è un contenitore personalizzato del disco Z (il dispositivo stesso da cui la ROM è stata clonata). Vedi la [Sezione di dumping nella Wiki](https://github.com/EKA2L1/EKA2L1/wiki/Dumping-the-ROM-and-ROFS) per capire come clonarla.
	- Il file potrebbe essere necessario solo su dispositivi S60v2. L'emulatore lo richiederà durante l'installazione, se ritiene che la ROM da sola non basti.
	
### Per S60v3 e superiore (5320, 5800, N97, dispositivi compatibili con N-Gage 2.0, ecc...)

Ci sono due metodi tra cui puoi scegliere:

- ROM e RPKG del dispositivo (come per S60v1 e S60v2)
- Il firmware del dispositivo selezionato. **Assicurati** che il firmware che hai ottenuto contenga anche un file VPL.

Al momento, per gli utenti interessati solo al N-Gage 2.0, il dispositivo Nokia 5320 è il più mantenuto e supportato a questo scopo.

## Installare un dispositivo

- Per prima cosa, compila o [scarica](https://12z1.com/download/) EKA2L1 per la piattaforma su cui vuoi utilizzare l'emulatore.

### Per PC (Windows, MacOS, Linux)

- Avvia l'emulatore da riga di comando con l'opzione **--help** se vuoi una lista dei comandi disponibili.
- Per installare un nuovo dispositivo, vai a *File/Install/Device*, o segui la finestra di installazione che viene mostrata al primo avvio dell'emulatore.

{% include figure image_path="/assets/quickstart/en/device_dialog.png" alt="The device install dialog" caption="The device install dialog" %}

- In questa finestra:
	- Se hai preparato una ROM (con eventuale file RPKG), scegli il metodo di installazione **Device dump**, e clicca *Browse* per selezionare la ROM che hai preparato. Se la ROM da sola non basta, ti verrà fatto selezionare il file RPKG.
	{% include figure image_path="/assets/quickstart/en/device_dialog_with_rpkg.png" alt="Nel campo RPKG appare selezionata la ROM 5320" caption="Nel campo RPKG appare selezionata la ROM 5320" %}

	- Se hai preparato un firmware, scegli il metodo di installazione **Firmware (VPL)**. Il campo ROM verrà chiamato VPL, e potrai cliccare *Browse* per scegliere il file VPL che era abbinato al firmware.
	{% include figure image_path="/assets/quickstart/en/device_dialog_vpl.png" alt="La finestra di installazione VPL" caption="La finestra di installazione VPL" %}

	- **Nota**: È meglio che il percorso dei file non contenga caratteri Unicode o speciali. Gli sviluppatori stanno cercando di rendere l'emulatore più compatibile con percorsi Unicode, ma per ora l'emulatore avrà dei problemi con essi.

- Dopo che hai compilato tutti i campi, premi *Install*. Se vuoi annullare l'installazione, premi il tasto *Cancel*, a fianco di *Install*.
	- Per il metodo di installazione **Device dump**, aspetta che la barra del progresso si riempia e che spunti una finestra che confermi il successo di installazione.
	- Per il metodo di installazione **Firmware (VPL)**, potrebbe essere necessario scegliere una variante del firmware. Di solito le opzioni sono correlate alla regione del dispositivo e al suo stile (nero, rosso...), e non dovrebbe avere molta importanza. Dopo di che, il processo è identico a quello del metodo **Device dump**.

{% include figure image_path="/assets/quickstart/en/device_dialog_install_success.png" alt="Finestra del successo di installazione" caption="Finestra del successo di installazione" %}

- Se raggiungi la finestra qui sopra, allora hai installato un dispositivo con successo.

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
