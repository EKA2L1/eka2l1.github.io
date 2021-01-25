---
layout: single
title:  "32-bit Android đã được hỗ trợ!"
date:   2021-01-25 21:30:00 +0700
categories: jekyll update
---

Phiên bản mới nhất của EKA2L1 đã thêm hỗ trợ cho nền tảng **Android 32-bit**. Hãy tải xuống APK như thường tại phần [**Download**]({{ site.baseurl_root }}/vi/download)

**Xin lưu ý:**
- Hiện tại, chỉ có ứng dụng S60v1 và S60v3 được hỗ trợ trên bản 32-bit này.
- Không phải tất cả thiết bị 32-bit Android có thể chạy giả lập này, cho dù yêu cầu cấu hình khá thấp.

Hãy xem *cấu hình tối thiểu* cho Android ở trang [**Quickstart**]({{ site.baseurl_root }}/vi/quickstart)

[**CPU-Z**]((https://play.google.com/store/apps/details?id=com.cpuid.cpu_z)) được khuyến nghị sử dụng để lấy cấu hình điện thoại, sau đó đối chiếu với cấu hình tối thiểu nhé.

### Vài lời ngoài lề

Trước đó, hỗ trợ cho bản 32-bit thiếu vắng do không có giả lập ARM CPU nào mà hỗ trợ 32-bit ARM cả.

Giả lập CPU chúng tôi đang dùng là [(Dynarmic)](https://github.com/MerryMage/Dynarmic), hiện chỉ hỗ trợ **64-bit ARM (AArch64)** và **x86_64**.
Gần đây chúng tôi viết giả lập CPU riêng cho 32-bit, không nhanh nhưng đủ ổn. Duyên phận cho ai đang dùng 32-bit thật.