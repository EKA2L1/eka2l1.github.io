---
layout: single
title:  "已经支持32位的Android系统了!"
date:   2021-01-25 21:30:00 +0700
categories: jekyll update
---

最新版本的EKA2L1增加了对 **32位 Android** 平台的支持. 请您像往常一样 [**下载APK**]({{ site.baseurl_root }}/download) section.

**请注意:**
- At the moment, only S60v3 and S60v1 apps are supported.
- Not all 32-bit Android devices can run the emulator, although the expected specs are quite low.
Please check the *minimum requirements* for Android at [**Quickstart**]({{ site.baseurl_root }}/quickstart) page.

推荐使用 [**CPU-Z**](https://play.google.com/store/apps/details?id=com.cpuid.cpu_z) 获取您的手机硬件信息来了解是否达到了最低要求.

**小提示:**

Previously, the support was absent because there was no ARM CPU emulator present that support the **32-bit ARM** architecture.

The CPU emulator we are using [(Dynarmic)](https://github.com/MerryMage/Dynarmic) currently on support **64-bit ARM (AArch64)** and **x86_64** architecture.
We recently write our own CPU emulator, it's not the most optimised, but it seems to perform decently.
