Per favore, utilizza la *Tabella dei Contenuti* a destra per navigare tra le sezioni che ti interessano.

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

Ci sono due metodi tra i quali puoi scegliere:

- ROM e RPKG del dispositivo (come per S60v1 e S60v2)
- Il firmware del dispositivo selezionato. **Assicurati** che il firmware che hai ottenuto contenga anche un file VPL.

Al momento, per gli utenti interessati solo al N-Gage 2.0, il dispositivo Nokia 5320 è il più mantenuto e supportato a questo scopo.

## Installare un dispositivo

- Per prima cosa, compila o [scarica](https://12z1.com/download/) EKA2L1 per la piattaforma su cui vuoi utilizzare l'emulatore.

### Su PC (Windows, MacOS, Linux)

- Avvia l'emulatore da riga di comando con l'opzione **--help** se vuoi una lista dei comandi disponibili.
- Per installare un nuovo dispositivo, vai a *File/Installa/Dispositivo*, o segui la finestra di installazione che viene mostrata al primo avvio dell'emulatore.

{% include figure image_path="/assets/quickstart/en/device_dialog.png" alt="La finestra di installazione del dispositivo" caption="La finestra di installazione del dispositivo" %}

- In questa finestra:
	- Se hai preparato una ROM (con eventuale file RPKG), scegli il metodo di installazione **Dump dispositivo**, e clicca *Sfoglia* per selezionare la ROM che hai preparato. Se la ROM da sola non basta, ti verrà chiesto il file RPKG.
	{% include figure image_path="/assets/quickstart/en/device_dialog_with_rpkg.png" alt="Nel campo RPKG appare selezionata la ROM 5320" caption="Nel campo RPKG appare selezionata la ROM 5320" %}

	- Se hai preparato un firmware, scegli il metodo di installazione **Firmware (VPL)**. Il campo ROM verrà chiamato VPL, e potrai cliccare *Sfoglia* per scegliere il file VPL che era abbinato al firmware.
	{% include figure image_path="/assets/quickstart/en/device_dialog_vpl.png" alt="La finestra di installazione VPL" caption="La finestra di installazione VPL" %}

	- **Nota**: È meglio che il percorso dei file non contenga caratteri Unicode o speciali. Gli sviluppatori stanno cercando di rendere l'emulatore più compatibile con percorsi Unicode, ma per ora l'emulatore avrà dei problemi con essi.

- Dopo che hai compilato tutti i campi, premi *Installa*. Se vuoi annullare l'installazione, premi il tasto *Annulla*, a fianco di *Installa*.
	- Per il metodo di installazione **Dump dispositivo**, aspetta che la barra del progresso si riempia e che spunti una finestra che confermi il successo di installazione.
	- Per il metodo di installazione **Firmware (VPL)**, potrebbe essere necessario scegliere una variante del firmware. Di solito le opzioni sono correlate alla regione del dispositivo e al suo stile (nero, rosso...), e non dovrebbe avere molta importanza. Dopo di che, il processo è identico a quello del metodo **Dump dispositivo**.

{% include figure image_path="/assets/quickstart/en/device_dialog_install_success.png" alt="Finestra del successo di installazione" caption="Finestra del successo di installazione" %}

- Se raggiungi la finestra qui sopra, allora hai installato un dispositivo con successo.

### Su Android

- Al primo avvio dell'emulatore ti viene mostrata una finestra di installazione del dispositivo. Per accedere rapidamente alla **Gestione Dispositivi**, premi *Installa*

{% include figure image_path="/assets/quickstart/en/android_device_install_request.jpg" alt="La finestra di installazione" caption="La finestra di installazione" %}

- Se la finestra non appare, premi i tre puntini in alto a destra sul tuo schermo, e scegli **Dispositivi**

{% include figure image_path="/assets/quickstart/en/android_devices_activity.jpg" alt="Schermata dei dispositivi su Android" caption="Schermata dei dispositivi su Android" %}

- In questa finestra:
 	- Se hai preparato una ROM (con eventuale file RPKG), scegli il metodo di installazione **Dump dispositivo**, e clicca il tasto *ROM* per selezionare la ROM che hai preparato. Se la ROM da sola non basta, ti verrà chiesto il file RPKG.
 	
	- Se hai preparato un firmware, scegli il metodo di installazione **Firmware (VPL)**. Il tasto ROM verrà chiamato VPL, e potrai cliccarlo per scegliere il file VPL che era abbinato al firmware.

	{% include figure image_path="/assets/quickstart/en/android_device_all_choosen.jpg" alt="Tutti i percorsi file sono selezionati" caption="Tutti i percorsi file sono selezionati" %}

- Dopo che avrai selezionato tutti i percorsi file, premi *Installa*. L'unico modo per annullare l'operazione è uscire dall'app. Non sono necessarie ulteriori azioni, una piccola notifica toast ti mostrerà l'esito dell'installazione.

{% include figure image_path="/assets/quickstart/en/android_new_device_appears.jpg" alt="Il nuovo dispositivo appare dopo l'installazione" caption="Il nuovo dispositivo appare dopo l'installazione" %}

- **Nota**: Per Android 11 e superiore, l'emulatore potrebbe rallentare notevolmente durante l'aggiunta di un dispositivo, perchè Google limita l'accesso ai file esterni alla cartella privata dell'app (e le operazioni con i file sono lentissime). Stiamo ancora ricercando una soluzione valida.

Se riscontri un errore durante l'installazione, per favore visita il server [Discord](https://discord.gg/5Bm5SJ9) per ricevere supporto.

## Installa un pacchetto (SIS)

### Nota importante

- È consigliabile installare prima un dispositivo, e impostare il dispositivo di destinazione su cui installare il pacchetto SIS, prima di procedere.

	- Questo è cruciale per i pacchetti N-Gage 2.0, che dipendono dal dispositivo attivo al momento dell'installazione per estrarre i file di configurazione adatti.

### Su PC

- Vai a *File/Installa/Pacchetto* e scegli il SIS che vuoi installare.


### Su Android

- Premi sul **grande tasto ``+``** in basso a destra sul tuo schermo, nella lista di app principale, e scegli il SIS che vuoi installare.

# Gestire i dispositivi

L'emulatore permette ai propri utenti di installare più di un dispositivo, e supporta il passaggio da un dispositivo all'altro. È indispensabile se vuoi usare applicazioni su piattaforme differenti *(S60v1, S60v3)* senza dover separare le istanze dell'emulatore o le cartelle dei dati.

## Su PC (Windows, MacOS, Linux)

Vai a *File/Impostazioni*, e scegli la scheda *Sistema*. La sezione *Dispositivi* contiene una lista dei dispositivi installati.

{% include figure image_path="/assets/quickstart/en/device_manager.png" alt="Sezione di gestione dispositivi" caption="Sezione di gestione dispositivi" %}

- Clicca il menù a tendina e scegli il dispositivo che vuoi utilizzare. I cambiamenti saranno salvati istantaneamente.

- Puoi anche rinominare i dispositivi per una gestione più semplice. Clicca il tasto **Rinomina** e inserisci il nuovo nome nella piccola finestra che si aprirà.

- Usa **Ricarica dispositivi** per rilevare i dispositivi installati che non appaiono nel menù a tendina.

- Usa **Convalida il dispositivo corrente** per avviare una scansione di eventuali errori nel dispositivo e coreggerli, per rendere il dispositivo eseguibile sulla piattaforma. Se il dispositivo continua a non avviarsi, significa che non è ancora supportato o ci sono altri errori. Puoi contattarci per ottenere altre informazioni.

## Su Android

La schermata con la quale si installano i dispositivi funge anche da gestore dispositivi. Diamogli ancora un'occhiata.

{% include figure image_path="/assets/quickstart/en/android_new_device_appears.jpg" alt="Schermata dispositivi" caption="Schermata dispositivi" %}

- Premi il menù a tendina cerchiato in rosso e scegli il dispositivo che vuoi utilizzare.  I cambiamenti saranno salvati istantaneamente.

- Puoi anche rinominare i dispositivi per una gestione più semplice. Clicca il tasto **Rinomina** e inserisci il nuovo nome nella piccola finestra che si aprirà.

- Al momento non è possibile convalidare un dispositivo come su PC.

# Cambiare la cartella dei dati

**Nota:** Questa operazione è supportata solo su PC. Qualsiasi errore prodotto da questa operazione su Android non sarà da noi supportato.

Di default, EKA2L1 salva i dati nella cartella **data**, che è nella stessa cartella dell'eseguibile *(eka2l1_qt.exe)*. Però, se non hai abbastanza spazio o vuoi spostarla in una posizione più duratura, puoi seguire questi semplici passi:

1. Sposta la cartella dati corrente nella posizione che preferisci. **Assicurati** che l'emulatore sia chiuso.

2. Cambia il percorso della cartella salvato nell'emulatore.

	- Con l'interfaccia grafica: Vai a *File/Impostazioni/Generale*. La sezione **Dati** apparirà in alto, premi il tasto **Sfoglia** per selezionare il nuovo percorso, poi l'emulatore chiederà di essere riavviato. Dopo di che, il percorso dei dati verrà cambiato.
	
	{% include figure image_path="/assets/quickstart/en/change_data_folder_pc.png" alt="Sezione impostazioni dei dati" caption="Sezione impostazioni dei dati" %}

	- Da file *config.yml*: trovi questo file nella stessa cartella del file eseguibile EKA2L1. Cambia la variabile *data-storage* nel file YAML inserendo il nuovo percorso da te selezionato.
	
# Altre domande

## Dove posso trovare altre guide?

Questa guida è solo un'introduzione, e non fornirà dettagli su ulteriori usi specifici. Si prega di visitare [la wiki dell'emulatore](https://eka2l1.miraheze.org/wiki/Main_Page) per altre guide e informazioni.

## Non riesco a ottenere o installare file ROM/RPKG, fallisce sempre!

Ti consigliamo di visitare il server [Discord](https://discord.gg/5Bm5SJ9) per ricevere supporto.

Puoi usare un pacchetto già configurato seguendo le istruzioni della [wiki](https://eka2l1.miraheze.org/wiki/How_To_Use_The_Preconfigured_Pack), però è un file ingombrante. Se devi utilizzare solo un'app o gioco specifico, installa un dispositivo manualmente seguendo le istruzioni più in alto.

## Avete dei video che mostrano i passaggi?

Non ne abbiamo, ma in rete esistono già molti video che spiegano perfettamente come fare. Consigliamo caldamente di fare una ricerca su YouTube, perché in effetti l'emulatore può essere difficile da inizializzare.
