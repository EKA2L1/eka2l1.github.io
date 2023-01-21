---
layout: single
title:  "Android a 32-bit ora è supportato!"
date:   2021-01-25 21:30:00 +0700
categories: jekyll update
---

La versione più recente di EKA2L1 ha aggiunto il supporto alla piattaforma **Android 32-bit**. Per ottenerlo scarica l'APK dalla sezione [**Download**]({{ site.baseurl_root }}/download).

**Per favore, nota che:**
- Al momento, solo le app S60v3 e S60v1 sono supportate.
- Non tutti i dispositivi Android 32-bit possono far girare l'emulatore, anche se i requisiti sono abbastanza bassi.
Per favore, controlla i *requisiti minimi* per Android nella pagina di [**Introduzione**]({{ site.baseurl_root }}/quickstart).

Si consiglia di usare [**CPU-Z**](https://play.google.com/store/apps/details?id=com.cpuid.cpu_z) per ottenere le specifiche del tuo telefono e confrontarle con i requisiti minimi.

### Alcune note minori

In precedenza, il supporto era assente perché non esisteva un emulatore per CPU ARM che supportasse l'architettura **32-bit ARM**

L'emulatore CPU che stiamo usando [(Dynarmic)](https://github.com/MerryMage/Dynarmic) al momento supporta solo le architetture **64-bit ARM (AArch64)** e **x86_64**.
Recentemente abbiamo scritto il nostro emulatore CPU. Non è il più ottimizzato, ma sembra performare in modo decente.
