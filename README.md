# 🏠☁️ Host/Game Device App

> Aplikasi peranti sasaran yang menjalankan permainan dan menerima input kawalan dari Game Controller. Boleh berjalan pada peranti fizikal atau Cloud Phone.

## 📋 Penerangan
Aplikasi ini adalah bahagian **Host** dalam sistem Scrcpy Game Controller. Ia dipasang pada peranti sasaran (Android TV, tablet, telefon kedua, atau Cloud Phone) dan bertindak sebagai pelayan yang menjalankan permainan sebenar.

## ✨ Ciri-ciri
- 🎮 Menjalankan permainan Android yang sebenar
- 📡 Server Scrcpy untuk menerima sambungan dari Controller
- 🎬 Menstrim video & audio berkualiti tinggi ke peranti Controller
- ⚡ Memproses input sentuh dengan latensi rendah
- ☁️ Menyokong penuh persekitaran Cloud Phone
- 🔒 Tidak memerlukan root

## 🚀 Cara Deploy di GitHub

### 1. Muat Naik Kod ke GitHub
```bash
git init
git add .
git commit -m "Initial commit: Host/Game Device App"
git branch -M main
git remote add origin https://github.com/USERNAME/host-game-device-app.git
git push -u origin main
```

### 2. GitHub Actions Auto-Build
Fail `.github/workflows/build.yml` sudah sedia dikonfigurasi. Ia akan:
- ✅ Build APK secara automatik pada setiap `push` ke branch `main`
- ✅ Muat naik APK sebagai **Artifact**
- ✅ Auto-cipta **GitHub Release** untuk tag versi `v*`

### 3. Cara Deploy ke Cloud Phone
1. Dapatkan APK dari GitHub Actions Artifact atau Release
2. Muat naik APK ke panel kawalan Cloud Phone anda
3. Pasang pada instance Cloud Phone
4. Aktifkan ADB Debugging dalam tetapan Cloud Phone
5. Catat alamat IP awam + port yang diberikan

## 📱 Cara Guna (Peranti Fizikal)
1. Pasang APK pada peranti sasaran
2. Aktifkan **USB Debugging** atau **ADB over network**
3. Pastikan peranti disambung ke rangkaian yang sama dengan Controller
4. Sedia menerima sambungan dari Game Controller App

## ☁️ Cara Guna (Cloud Phone)
1. Pasang APK pada instance Cloud Phone
2. Aktifkan ADB melalui panel perkhidmatan Cloud Phone
3. Pasang permainan yang dikehendaki
4. Gunakan alamat IP awam untuk menyambung dari Controller

## 🔗 Berkaitan
- [Game Controller App](../game-controller-app/) — Aplikasi pengawal
- [Dokumentasi Sistem](../docs/) — Panduan lengkap
- [Panduan Cloud Phone](../docs/cloud-phone-setup.md) — Penyediaan Cloud Phone terperinci
