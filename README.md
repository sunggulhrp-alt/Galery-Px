# Galery Px — Android test project 0.1.1

Proyek Android native untuk pengujian pada Vivo V2111 / Android 12.

## Isi proyek
- Halaman awal galeri.
- Akses kalkulator rahasia melalui tekan lama judul Galeri.
- PIN 4–8 digit.
- Brankas lokal dengan AES-256-GCM dan kunci Android Keystore.
- Impor/ekspor file melalui Android document picker.
- Pintasan untuk membuka Telegram, WhatsApp, dan Facebook yang terpasang.
- Ikon launcher Galery Px disertakan pada resource Android.

## Batasan penting
- Tombol sembunyikan hanya menyembunyikan pintasan dari daftar di aplikasi ini. Aplikasi asli tetap terlihat di launcher dan Pengaturan Android.
- Proyek ini belum mengkloning Telegram, WhatsApp, atau Facebook. Kloning nyata memerlukan mesin virtualisasi terpisah dan uji kompatibilitas; tidak dijanjikan berfungsi pada build ini.
- Jangan gunakan sebagai satu-satunya salinan file penting. Menghapus data/aplikasi dapat menghilangkan file brankas lokal karena kunci disimpan di Android Keystore.
- Uji dahulu dengan salinan foto/video yang tidak penting.

## Build APK melalui GitHub Actions
1. Unggah isi ZIP ini ke root repositori GitHub, bukan folder ZIP sebagai satu subfolder.
2. Buka Actions.
3. Jalankan workflow `Build Galery Px APK`.
4. Unduh artifact `Galery-Px-debug-apk` setelah build berhasil.

## Konfigurasi build
- JDK 17
- Gradle 8.9
- Android SDK platform 35
- Android Gradle Plugin 8.7.3
