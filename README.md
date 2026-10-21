# Titto Journal XAUUSD (APK)

## Cara 1 - GitHub Actions (tanpa install apa pun)
1. Buat repo GitHub baru, upload semua isi folder ini, branch `main`.
2. Buka tab Actions > "Build APK" (jalan otomatis saat push).
3. Setelah hijau, unduh artifact `tittotrader-journal-apk` -> `app-debug.apk`.
4. Kirim ke HP, aktifkan "Install dari sumber tidak dikenal", install.

## Cara 2 - Android Studio
1. `npm install && npm run build && npx cap sync android`
2. `npx cap open android` > Build > Build APK(s).

Catatan: data jurnal disimpan di localStorage WebView di HP (tidak sinkron antar perangkat; hilang jika app di-uninstall / data dihapus).
