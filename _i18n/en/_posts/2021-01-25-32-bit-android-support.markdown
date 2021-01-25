---
layout: single
title:  "32-bit Android is now supported!"
date:   2021-01-25 21:30:00 +0700
categories: jekyll update
---

The lastest version of EKA2L1 has added support for **32-bit Android** platform. Please proceed to download the APK as usual in [**Download**]({{ site.baseurl_root }}/download) section.

**Please take note,** not all 32-bit Android devices can run the emulator, although the expected specs are quite low.
Please check the *minimum requirements* for Android at [**Quickstart**]({{ site.baseurl_root }}/quickstart) page.

It's recommended to use [**CPU-Z**](https://play.google.com/store/apps/details?id=com.cpuid.cpu_z) to get your phone statistics and compare it with minimum requirements.

### Some small notes

Previously, the support was absent because there was no ARM CPU emulator present that support the **32-bit ARM** architecture.

The CPU emulator we are using [(Dynarmic)](https://github.com/MerryMage/Dynarmic) currently on support **64-bit ARM (AArch64)** and **x86_64** architecture.
We recently write our own CPU emulator, it's not the most optimised, but it seems to perform decently.
