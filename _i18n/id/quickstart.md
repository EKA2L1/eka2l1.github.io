Silakan gunakan *Daftar Isi* untuk menelusuri bagian yang Anda butuhkan.

# Persyaratan

## Untuk versi PC:

### Minimal

- **OS:** Menggunakan **64-bit OS**. Untuk **Windows**, Anda harus menggunakan dari *Windows 7* ke atas

- **Prosesor:** CPU 64-bit apa pun dari sekitar tahun 2007, mulai dari **Core 2 Duo E4300**

- **Memori:** RAM minimal 2GB

- **Kartu grafik:** Semua GPU yang kompatibel dengan OpenGL 3.1 atau lebih tinggi.

### Direkomendasikan

- **OS:** Menggunakan **64-bit OS**. Untuk **Windows**, disarankan untuk menggunakan *Windows 10*

- **Prosesor:** CPU Intel atau AMD apa pun dengan 4 inti ke atas

- **Memori:** RAM 4GB atau lebih

- **Kartu grafis:** Semua GPU yang kompatibel dengan OpenGL 3.3 atau lebih tinggi.

## Untuk versi Android:

### Minimal

- **OS:** Android 5.0 32-bit

- **Prosesor:** CPU ARMv7 atau yang lebih tinggi. **ARMv6 dan ke bawah tidak didukung!**

- **Memori:** RAM minimal 2GB

- **Kartu grafis:** Semua GPU yang kompatibel dengan OpenGL ES 3.0 atau lebih tinggi

### Direkomendasikan

- **OS:** Android 7.0 64-bit (32-bit bersifat eksperimental)

- **Prosesor:** CPU ARMv8

- **Memori:** RAM 4GB atau lebih

- **Kartu grafis:** Semua GPU yang kompatibel dengan OpenGL ES 3.2 atau lebih tinggi

# Persiapan

## Berkas yang harus disiapkan

### Untuk perangkat S60v1 dan S60v2 (N-Gage, N70, dll...)

- ROM perangkat

- Berkas RPKG

- Ini adalah wadah khusus dari drive Z (perangkat yang sama dengan tempat ROM didumping). Lihat [bagian Dumping di Wiki](https://github.com/EKA2L1/EKA2L1/wiki/Dumping-the-ROM-and-ROFS) untuk mengetahui cara dumping-nya

- File mungkin hanya diperlukan dengan perangkat S60v2. Emulator akan menanyakannya saat instalasi jika hanya mendeteksi ROM saja tidak cukup.

### Untuk S60v3 dan yang lebih tinggi (perangkat yang kompatibel dengan 5320, 5800, N97, N-Gage 2.0, dll...)

Ada dua opsi yang bisa Anda pilih:

- ROM dan RPKG perangkat (sama seperti S60v1 dan S60v2)

- Sebuah firmware dari perangkat target. **Pastikan** firmware yang Anda dapatkan juga memiliki file VPL.

Saat ini, untuk pengguna yang hanya tertarik dengan N-Gage 2.0, perangkat Nokia 5320 adalah perangkat yang paling terjaga dan didukung untuk pilihan ini.

## Instal perangkat

- Pertama, buat atau [unduh](https://12z1.com/download/) EKA2L1 untuk platform target Anda ingin menjalankan emulator.

### Untuk PC (Windows, MacOS, Linux)

- Luncurkan emulator dengan opsi command line **--help** jika Anda ingin berinteraksi melalui command line dan memerlukan list of command.

- Untuk menginstal perangkat baru, buka *File/Instal/Perangkat*, atau ikuti dialog yang meminta Anda untuk menginstal perangkat yang muncul saat pertama kali menjalankan emulator.

{% include figure image_path="/assets/quickstart/en/device_dialog.png" alt="Dialog pemasangan perangkat" caption="Dialog pemasangan perangkat" %}

- Dalam dialog ini:

- Jika sudah menyiapkan ROM (dan RPKG jika diperlukan), pilih metode instalasi **Device dump**, dan klik *Telusur* pertama untuk memilih ROM yang sudah disiapkan. Jika emulator mendeteksi bahwa ROM tidak cukup, browser file RPKG akan muncul.

{% include figure image_path="/assets/quickstart/en/device_dialog_with_rpkg.png" alt="Bidang RPKG muncul dengan 5320 ROM dipilih" caption="Bidang RPKG muncul dengan 5320 ROM dipilih" %}

- Jika sudah menyiapkan firmware, pilih metode instalasi **Firmware (VPL)**. Label ROM akan diubah namanya menjadi VPL, lalu Anda dapat mengeklik *Telusur* untuk memilih VPL yang disertakan dengan firmware.

{% include figure image_path="/assets/quickstart/en/device_dialog_vpl.png" alt="Dialog pemasangan VPL" caption="Dialog pemasangan VPL" %}

- **Catatan**: Sebaiknya path/jalur Anda tidak berisi Unicode atau karakter khusus lainnya, pengembang mencoba membuat emulator lebih kompatibel dengan jalur Unicode, tetapi untuk saat ini emulator tidak akan berfungsi dengan baik dengan jalur tersebut.

- Setelah Anda mengisi semua path/jalur, tekan *Install*. Jika Anda ingin membatalkan penginstalan, Anda dapat menekan tombol *Batal* di sebelah *Install*.

- Untuk metode penginstalan **Device dump**, Anda dapat menunggu bilah progres selesai dan dialog sukses muncul.

- Untuk metode **Firmware (VPL)**, Anda mungkin perlu memilih varian firmware. Ini biasanya terkait dengan wilayah/region perangkat dan variasi style-nya (hitam atau merah), dan seharusnya tidak terlalu menjadi masalah pada emulator. Setelah itu prosesnya sama dengan **Device dump**.

{% include figure image_path="/assets/quickstart/en/device_dialog_install_success.png" alt="Dialog sukses pemasangan" caption="Dialog sukses pemasangan" %}

- Jika Anda melihat dengan dialog di atas, maka itu berarti Anda telah selesai menginstal perangkat.

### Untuk Android

- Emulator yang dijalankan pertama kali akan menampilkan dialog yang meminta Anda untuk memasang perangkat. Tekan dialog *Instal*, untuk membuka **Pengelola perangkat** dengan cepat.

{% include figure image_path="/assets/quickstart/en/android_device_install_request.jpg" alt="Dialog pemasangan permintaan" caption="Dialog pemasangan permintaan" %}

- Jika dialog tidak muncul, tekan tiga titik di kanan atas layar Anda, lalu pilih **Devices**.

{% include figure image_path="/assets/quickstart/en/android_devices_activity.jpg" alt="Layar perangkat Android" caption="Layar perangkat Android" %}

- Di layar ini:

- Jika Anda telah menyiapkan ROM (dan RPKG jika diperlukan), pilih metode instalasi **Device dump**, dan tekan tombol *ROM* untuk memilih ROM yang telah Anda siapkan. Jika emulator mendeteksi bahwa ROM tidak cukup, browser file RPKG akan muncul.

- Jika sudah menyiapkan firmware, pilih metode instalasi **Firmware (VPL)**. Tombol ROM akan diganti namanya menjadi VPL, lalu Anda dapat mengklik tombol *VPL* untuk memilih VPL yang disertakan dengan firmware.

{% include figure image_path="/assets/quickstart/en/android_device_all_choosen.jpg" alt="Semua jalur file terisi" caption="Semua jalur file terisi" %}

- Setelah Anda mengisi semua jalur, tekan *Install*. Anda hanya dapat membatalkan operasi ini dengan keluar dari aplikasi, dan tidak perlu tindakan lebih lanjut sampai pemberitahuan bersulang kecil memberi tahu Anda bahwa penginstalan berhasil atau mengalami kegagalan.

{% include figure image_path="/assets/quickstart/en/android_new_device_appears.jpg" alt="Perangkat baru muncul setelah pemasangan" caption="Perangkat baru muncul setelah pemasangan" %}

- **Catatan**: Untuk Android 11 dan yang lebih baru, emulator mungkin mengalami pelambatan besar pada penginstalan perangkat, karena pembatasan yang diterapkan Google pada file di luar folder pribadi aplikasi (operasi file sangat lambat). Kami masih menemukan solusi yang cocok untuk emulator.

Jika Anda mengalami kegagalan selama penginstalan, silakan kunjungi server [Discord](https://discord.gg/5Bm5SJ9) untuk menerima dukungan.

## Instal paket (SIS)

### Catatan penting

- Harap dicatat bahwa sangat disarankan untuk menginstal perangkat/device terlebih dahulu dan mengubah ke perangkat/device target tempat Anda ingin menginstal SIS, sebelum melanjutkan langkah ini.

- Ini sangat penting untuk paket seperti N-Gage 2.0, yang bergantung pada perangkat aktif saat ini untuk mengekstrak file konfigurasi game yang sesuai.

### Untuk Komputer

- Buka *File/Instal/Paket* dan pilih SIS yang ingin Anda instal.

### Untuk Android

- Tekan tombol **big green ``+`` button** di kanan bawah layar utama (daftar aplikasi) dan pilih SIS yang ingin Anda pasang.

# Mengelola perangkat

Emulator memungkinkan pengguna untuk menginstal beberapa perangkat, dan juga mendukung peralihan antar perangkat. Ini diperlukan jika Anda ingin menggunakan aplikasi pada platform yang berbeda *(S60v1, S60v3)*, tanpa memerlukan instance emulator baru dengan folder data instance baru.

## Untuk PC (Windows, MacOS, Linux)

Buka *File/Settings*, dan pilih tab *System*. Bagian *Perangkat* mencantumkan semua perangkat yang terpasang.

{% include figure image_path="/assets/quickstart/en/device_manager.png" alt="Bagian pengelola perangkat" caption="Bagian pengelola perangkat" %}

- Tekan pada kotak kombo dan pilih perangkat yang ingin Anda jalankan. Perubahan akan segera diterapkan.

- Anda juga dapat mengganti nama perangkat untuk manajemen yang lebih mudah. Tekan tombol **Ubah nama** dan masukkan nama baru di dialog input kecil.

- Gunakan **Pindai ulang perangkat** untuk mendeteksi perangkat terpasang yang tidak muncul di kotak kombo.

- Gunakan **Validasi perangkat saat ini** untuk emulator untuk mendeteksi kesalahan apa pun pada perangkat dan memperbaikinya, agar perangkat dapat dijalankan di platform. Jika perangkat masih tidak berjalan, berarti belum didukung atau ada kesalahan lain, Anda dapat menghubungi kami untuk informasi lebih lanjut.

## Untuk Android

Layar sebelumnya tempat Anda memasang perangkat juga merupakan layar pengelola perangkat. Mari kita lihat lagi.

{% include figure image_path="/assets/quickstart/en/android_new_device_appears.jpg" alt="Layar perangkat" caption="Layar perangkat" %}

- Tekan kombo yang dilingkari merah dan pilih perangkat yang ingin Anda jalankan. Perubahan akan segera diterapkan.

- Anda juga dapat mengganti nama perangkat untuk manajemen yang lebih mudah. Tekan tombol **Ubah nama** dan masukkan nama baru di dialog input kecil.

- Saat ini tidak ada pindai ulang atau tombol untuk memvalidasi perangkat seperti di PC.

# Ubah direktori data

**Catatan:** Ini hanya didukung di PC. Kesalahan apa pun yang dihasilkan dengan melakukan ini di Android tidak akan didukung oleh kami.

Secara default, EKA2L1 menyimpan data dalam folder **data**, berada di lokasi yang sama dengan *(eka2l1_qt.exe)* yang dapat dieksekusi. Namun, jika ruang penyimpanannya tidak cukup atau Anda hanya ingin memindahkannya ke lokasi yang lebih persisten, Anda dapat melakukannya dengan mengikuti langkah-langkah berikut:

1. Pindahkan folder data saat ini ke lokasi pilihan Anda. **Pastikan** emulator ditutup.

2. Ubah jalur data emulator yang tersimpan.

- Dengan UI: Buka *File/Pengaturan/Umum*. Anda akan melihat bagian **Data** muncul di atas, tekan tombol **Telusur** untuk memilih lokasi baru, lalu emulator diminta untuk di-restart. Setelah itu, jalur penyimpanan data Anda berubah total.

{% include figure image_path="/assets/quickstart/en/change_data_folder_pc.png" alt="Bagian pengaturan data" caption="Pengaturan data" %}

- Dengan file *config.yml*: File ini berada di folder yang sama dengan file EKA2L1 dapat dieksekusi. Ubah variabel *penyimpanan data* di YAML ke jalur data baru yang Anda inginkan.

# Lebih banyak pertanyaan

## Di mana saya dapat menemukan lebih banyak panduan?

Panduan ini hanya berfungsi sebagai panduan memulai, dan tidak akan memberikan detail lebih lanjut tentang penggunaan spesifik lebih lanjut. Kunjungi [wiki emulator](https://eka2l1.miraheze.org/wiki/Main_Page) untuk panduan dan informasi lebih lanjut.

## Saya tidak bisa mendapatkan ROM/RPKG atau saya tidak bisa menginstal, selalu gagal!

Sebaiknya kunjungi [Discord](https://discord.gg/5Bm5SJ9) untuk mendapatkan dukungan.

Anda dapat menggunakan paket prakonfigurasi mengikuti instruksi di [wiki](https://eka2l1.miraheze.org/wiki/How_To_Use_The_Preconfigured_Pack), namun paket ini sangat besar, jika Anda hanya perlu memainkan game/aplikasi tertentu, instal perangkat satu per satu ikuti langkah di atas.

## Apakah Anda memiliki video yang divisualisasikan langkah demi langkah?

Kami tidak punya, tapi ada banyak video yang membuat instruksi sempurna. Sangat disarankan untuk melakukan pencarian di Youtube untuk video-video ini, karena kami akui pengaturan emulatornya cukup sulit.
