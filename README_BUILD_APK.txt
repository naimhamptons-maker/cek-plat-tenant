PANDUAN MENGUBAH MENJADI FILE .APK ANDROID
=========================================

Paket ini berisi aplikasi Cek Plat Kendaraan Tenant (Sheet TOWER A + Auto Sync Google Sheet + 100% Offline) yang sudah disiapkan untuk dibungkus menjadi file .APK Android.

PILIH SALAH SATU CARA BERIKUT (DARI YANG PALING MUDAH):

------------------------------------------------------------
CARA 1: TANPA INSTALL SOFTWARE (VIA WEBSITE2APK / APPGEYSER / WEBINTOAPP)
------------------------------------------------------------
1. Ekstrak file ZIP ini dan ambil folder `www` (berisi `index.html`, `manifest.json`, `icon.svg`).
2. Gunakan salah satu converter lokal HTML-ke-APK gratis:
   - WebIntoApp (https://www.webintoapp.com) -> Pilih "HTML / Local Files", upload isi folder `www`, beri nama "Cek Plat Tenant", lalu klik Make App & Download APK.
   - Website 2 APK Builder (di PC Windows) -> Pilih "Local HTML Website", arahkan Directory ke folder `www`, aktifkan izin Internet (untuk fitur Auto-Sync Google Sheet), lalu klik Generate APK.

------------------------------------------------------------
CARA 2: OTOMATIS DI CLOUD VIA GITHUB ACTIONS (100% GRATIS & RESMI)
------------------------------------------------------------
1. Buat repository baru di GitHub (https://github.com/new).
2. Upload seluruh isi folder dalam ZIP ini ke repository tersebut (termasuk folder `.github`).
3. Buka tab "Actions" di repository GitHub Anda -> klik "Build Android APK" -> klik "Run workflow".
4. Tunggu sekitar 3 menit hingga centang hijau, lalu unduh file `CekPlatTenant-Android-APK` yang berisi `app-debug.apk`.

------------------------------------------------------------
CARA 3: BUILD DI PC DENGAN CAPACITOR + ANDROID STUDIO
------------------------------------------------------------
1. Buka terminal/CMD di folder hasil ekstrak ZIP ini.
2. Jalankan perintah:
   npm install
   npx cap add android
   npx cap sync android
   npx cap open android
3. Di Android Studio, klik menu Build > Build Bundle(s) / APK(s) > Build APK(s).
