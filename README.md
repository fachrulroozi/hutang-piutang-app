# Hutang Piutang — Personal Web App

Aplikasi statis untuk mengisi template surat perjanjian hutang piutang, menyimpan draft di browser, dan mencetak PDF A4.

## File
- `index.html`: aplikasi utama.
- `manifest.webmanifest`: metadata agar dapat dipasang sebagai PWA.
- `service-worker.js`: cache offline setelah aplikasi pertama kali dibuka.
- `icon.svg`: ikon aplikasi.

## Deploy gratis dengan GitHub Pages
1. Buat repository GitHub baru bernama `hutang-piutang-app`.
2. Untuk GitHub Pages gratis, repository biasanya perlu **Public**. Jangan masukkan data pribadi atau dokumen hutang ke repository.
3. Upload seluruh file dalam folder ini ke root repository.
4. Buka **Settings → Pages**.
5. Pada **Build and deployment**, pilih **Deploy from a branch**, branch `main`, folder `/ (root)`, lalu Save.
6. Tunggu proses publikasi. GitHub akan menampilkan URL permanen, biasanya `https://USERNAME.github.io/hutang-piutang-app/`.

## Privasi
- Isi dokumen disimpan pada `localStorage` browser di perangkat yang sedang digunakan.
- Isi hutang, NIK, alamat, dan nominal tidak dikirim ke server oleh aplikasi ini.
- Jangan menyimpan data pribadi di source repository.
- Gunakan perangkat pribadi dan kunci layar. Backup PDF secara aman setelah dokumen final.

## Catatan
PWA/service worker membutuhkan HTTPS atau localhost. GitHub Pages menyediakan HTTPS. Aplikasi ini tidak memiliki login, sinkronisasi cloud, database, atau multi-user.
