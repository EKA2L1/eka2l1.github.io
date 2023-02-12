---

tata letak: tunggal

judul: "Android 32-bit sekarang didukung!"

tanggal: 25-01-2021 21:30:00 +0700

kategori: pembaruan jekyll

---

Versi terbaru EKA2L1 telah menambahkan dukungan untuk platform **32-bit Android**. Lanjutkan untuk mengunduh APK seperti biasa di bagian [**Download**]({{ site.baseurl_root }}/download).

**Mohon dicatat:**

- Saat ini, hanya aplikasi S60v3 dan S60v1 yang didukung.

- Tidak semua perangkat Android 32-bit dapat menjalankan emulator, meskipun spesifikasi yang diharapkan cukup rendah.

Periksa *persyaratan minimum* untuk Android di halaman [**Quickstart**]({{ site.baseurl_root }}/quickstart).

Sebaiknya gunakan [**CPU-Z**](https://play.google.com/store/apps/details?id=com.cpuid.cpu_z) untuk mendapatkan statistik ponsel Anda dan membandingkannya dengan persyaratan minimum.

### Beberapa catatan kecil

Sebelumnya, dukungan tidak ada karena tidak ada emulator CPU ARM yang mendukung arsitektur **32-bit ARM**.

Emulator CPU yang kami gunakan [(Dynarmic)](https://github.com/MerryMage/Dynarmic) saat ini mendukung arsitektur **64-bit ARM (AArch64)** dan **x86_64**.

Kami baru-baru ini menulis emulator CPU kami sendiri, ini bukan yang paling dioptimalkan, tetapi tampaknya berfungsi dengan baik.
