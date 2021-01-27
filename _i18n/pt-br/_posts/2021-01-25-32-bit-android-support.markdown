---
layout: single
title:  "Android de 32 bits agora é compatível!"
date:   2021-01-25 21:30:00 +0700
categories: jekyll update
---

A versão mais recente do EKA2L1 adicionou suporte para a plataforma ** Android de 32 bits **. Faça o download do APK normalmente na seção [**Download**]({{ site.baseurl_root }}/download).

**Por favor, leve em consideração:**
- No momento, apenas aplicativos S60v3 e S60v1 são compatíveis.
- Nem todos os dispositivos Android de 32 bits podem executar o emulador, embora os requisitos especificados sejam relativamente baixos.
Por favor, verifique os *requisitos mínimos* para Android na página [**Requisitos e instalação**]({{ site.baseurl_root }}/quickstart).

É recomendado usar o aplicativo [** CPU-Z **](https://play.google.com/store/apps/details?id=com.cpuid.cpu_z) para obter as especificações do seu dispositvo e compará-las com os requisitos mínimos.

### Algumas notas extras

Anteriormente, o suporte estava ausente porque não havia nenhum emulador de CPU ARM presente que suportasse a arquitetura **ARM de 32 bits**.

O emulador de CPU que estamos usando [(Dynarmic)](https://github.com/MerryMage/Dynarmic) atualmente oferece suporte para **ARM de 64 bits (AArch64)** e arquitetura **x86_64**.
Recentemente, escrevemos nosso próprio emulador de CPU, não é o mais otimizado, mas parece ter um desempenho decente.
