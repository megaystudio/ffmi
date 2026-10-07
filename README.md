# FFMI - Feed Formulation & Manufacturing Intelligence (Web) v1.1.1

Aplikasi web statis (tanpa server, tanpa build). Data pengguna tersimpan di browser masing-masing (localStorage) dan tidak dikirim ke server.

## Deploy ke GitHub Pages
1. Buat repository baru di GitHub (mis. `ffmi`).
2. Upload SELURUH isi folder ini (index.html, sw.js, manifest.webmanifest, icons/, download/, .nojekyll) ke root repository.
   JANGAN upload `keygen.js` - itu alat penjual.
3. Settings > Pages > Source: "Deploy from a branch" > Branch: `main` / `/ (root)` > Save.
4. Tunggu 1-2 menit. Alamat: `https://<username>.github.io/<nama-repo>/`

## Mode Demo dan Premium
- Web (tab browser) dan aplikasi terinstal (PWA): selalu Demo, kolom kode akses Premium tidak ditampilkan.
- File unduhan `FFMI.html` dibuka offline: Demo, atau Premium bila kode akses diaktifkan.
- Paket unduhan: `download/FFMI-offline.zip` (FFMI.html + BACA-DULU.txt).
- Pembatasan ini di sisi browser: cukup untuk pengguna umum, bukan keamanan kuat.

## User Manual
Manual ada di dalam aplikasi (menu Panduan, juga bisa dibuka dari layar login). Isinya ada di konstanta `MAN` dan `CHANGELOG` dalam `index.html`.

## CHECKLIST SETIAP UPDATE (wajib)
1. Ubah aplikasi di `index.html`.
2. Perbarui bagian terkait di `MAN` (kedua bahasa: id dan en) dan tambah entri baru di `CHANGELOG`.
3. Naikkan `APP_VER` dan `APP_DATE` di `index.html`, dan `VERSION` di `sw.js` (mis. `ffmi-1.1.2`).
4. Buat ulang `download/FFMI-offline.zip`: salin `index.html` menjadi `FFMI.html`, zip bersama `BACA-DULU.txt`.
5. Update judul versi di README ini, lalu commit dan push.

## Catatan
- Data terikat ke browser dan alamat/berkas yang dipakai. Pindah perangkat lewat Backup lalu Restore (Premium).
- Data hilang jika data situs browser dibersihkan: ingatkan pengguna untuk Backup berkala.
