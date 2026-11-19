# Island Survival 3D — HD Beach Adventure

Game petualangan bertahan hidup 3D dengan grafis HD (Three.js PBR, ACES Filmic Tone Mapping, Soft Shadows, ombak laut animasi, siklus siang-malam dinamis, crafting 3D, serta kontrol PC dan sentuh/HP).

## Daftar File (Siap Unggah ke GitHub)
- `index.html` — Kode utama game 3D lengkap (HTML + CSS + Three.js + Web Audio API)
- `icon-512.png`, `icon-192.png`, `apple-touch-icon.png`, `favicon.png`, `splash-1024.png` — Paket logo & ikon aplikasi lengkap (PWA, iOS/Android, Browser, dan Launcher APK)
- `manifest.json` & `sw.js` — Konfigurasi PWA agar bisa di-install di HP lengkap dengan ikon
- `package.json` & `capacitor.config.json` — Konfigurasi Capacitor 6 untuk build APK Android
- `deploy-pages.yml` — Workflow GitHub Actions untuk publikasi ke GitHub Pages
- `build-apk.yml` — Workflow GitHub Actions untuk kompilasi APK Android (Java 21 + Android SDK + ikon launcher otomatis)

## Cara Upload & Jalankan di GitHub (Lewat Browser HP/PC)
1. Buat repositori baru di GitHub (misalnya `island-survival-3d`), pilih **Public**.
2. Ekstrak file ZIP ini, lalu klik **Add file -> Upload files** di GitHub dan unggah semua file kode dan logo PNG sekaligus.
3. **Untuk GitHub Pages (Main Langsung di Browser):**
   - Klik **Add file -> Create new file**, ketik nama file `.github/workflows/deploy-pages.yml`, lalu tempel isi dari `deploy-pages.yml`.
   - Buka **Settings -> Pages -> Source: GitHub Actions**, tunggu workflow selesai, lalu buka link game-mu!
4. **Untuk Build APK Android (Opsional):**
   - Buat file `.github/workflows/build-apk.yml` menggunakan cara yang sama dan tempel isi dari `build-apk.yml`.
   - Buka tab **Actions -> Build Android APK**, unduh file `island-survival-3d-apk` setelah selesai.
