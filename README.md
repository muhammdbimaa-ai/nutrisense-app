# NutriSense - Aplikasi Pelacak Nutrisi

Aplikasi web (HTML tunggal) yang dibungkus menjadi aplikasi Android dengan Capacitor.

## Isi proyek
- `www/` : aplikasi (index.html, ikon)
- `.github/workflows/build-apk.yml` : pembuat APK di cloud GitHub
- `package.json`, `capacitor.config.json`

## Cara build APK di GitHub
1. Buat repository GitHub baru (atau pakai yang ada).
2. Upload **isi** folder ini ke root repository (jangan upload ZIP-nya).
   Pastikan terlihat: `www/index.html`, `.github/workflows/build-apk.yml`, `package.json`.
3. Commit ke branch `main`.
4. Buka tab **Actions** -> **Build APK** -> **Run workflow**.
5. Tunggu centang hijau, lalu unduh artifact **Workout-APK** (nama artifact tetap Workout-APK; isinya app-debug.apk).
6. Install `app-debug.apk` di HP Android.

## Catatan
- Data disimpan di localStorage HP (tidak hilang saat aplikasi ditutup).
- Untuk backup, gunakan fitur ekspor CSV/PDF di tab Mingguan.
- Ikon default (hijau dengan huruf N) bisa diganti dengan mengganti `www/icon-192.png` dan `www/icon-512.png`.