---
layout: single
title:  "已经支持32位的Android系统了!"
date:   2021-01-25 21:30:00 +0700
categories: jekyll update
---

最新版本的EKA2L1增加了对 **32位 Android** 平台的支持. 请您像往常一样 [**下载APK**]({{ site.baseurl_root }}/download) .

**请注意:**
- 目前只支持S60v3和S60v1应用程序。
- 并不是所有的32位Android设备都能运行模拟器，尽管预期的规格很低。
要了解 *最低要求*  请转到 [**快速开始**]({{ site.baseurl_root }}/quickstart) page.

推荐使用 [**CPU-Z**](https://play.google.com/store/apps/details?id=com.cpuid.cpu_z) 获取您的手机硬件信息来了解是否达到了最低要求.

**小提示:**
在此之前，由于没有支持**32位ARM**体系结构的ARM CPU模拟器，因此不支持此功能。.

我们正在使用[(Dynarmic)](https://github.com/MerryMage/Dynarmic) 的CPU模拟器，目前支持**64位ARM（AARCH64）**和**x86_64**体系结构.
我们最近自制了CPU模拟器，它没有经过优化，但运行效果很好。
