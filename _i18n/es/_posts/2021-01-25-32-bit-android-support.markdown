---
layout: single
title:  "¡Ahora Android de 32-bit es soportado!"
date:   2021-01-25 21:30:00 +0700
categories: jekyll update
---
 
La última versión de EKA2L1 ha agregado soporte para **Android de 32 bits**. Puede descargar la APK como de costumbre en la sección [**Descargas**]({{ site.baseurl_root }}/download).

**Por favor tome en cuenta:**
- Por el momento, solo aplicaciones de S60v3 y S60v1 estan soportadas.
- No todos los dispositivos Android de 32-bit soportan el emulador, aunque los requisitos sean relativamente bajos.
Por favor cheque los *requisitos mínimos* para android en la sección [**Requisitos e instalación**]({{ site.baseurl_root }}/quickstart).

Se recomienda utilizar [**CPU-Z**](https://play.google.com/store/apps/details?id=com.cpuid.cpu_z) para ver las espeficicaciones de su telefono mobil y compararlas con los
requisitos mínimos.

### Algunas notas extra

Previamente, no había soporte porque no había un emulador de ARM CPU que soportara la arquitectura de **32-bit ARM**.

El emulador de CPU [(Dynarmic)](https://github.com/MerryMage/Dynarmic) que estamos utilizando actualmente soporta las arquitecturas de 
**64-bit ARM (AArch64)** y **x86_64**.
De manera reciente creamos nuestro propio emulador de CPU, y aunque no esta muy optimizado, parece que funciona decentemente.
