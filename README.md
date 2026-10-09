# FFMI - Feed Formulation & Manufacturing Intelligence (Web) v1.3.0

Aplikasi web statis (tanpa server, tanpa build). Data pengguna tersimpan di browser masing-masing (localStorage) dan tidak dikirim ke server.
Sumber aplikasi: FFMI.html versi offline lengkap (diperbarui 2 Okt 2026) dengan revisi 1.3.0 (9 Okt 2026) + lapisan web (PWA, pembatasan Premium, User Manual, versi).

## Deploy / update di GitHub Pages
1. Ekstrak ZIP ini. Upload SELURUH isinya ke root repository (timpa file lama): index.html, sw.js, manifest.webmanifest, README.md, .nojekyll, icons/, download/.
   JANGAN upload `keygen.js` - itu alat penjual.
2. Settings > Pages > Source: "Deploy from a branch" > `main` / `/ (root)` > Save (cukup sekali).
3. Tunggu 1-3 menit, lalu buka `https://<username>.github.io/<nama-repo>/`. Header harus menampilkan versi v1.3.0.

## Mode Demo dan Premium
- Web (tab browser) dan aplikasi terinstal (PWA): selalu Demo, kolom kode akses Premium tidak ditampilkan.
- File unduhan `FFMI.html` dibuka offline: Demo, atau Premium bila kode akses diaktifkan.
- Paket unduhan: `download/FFMI-offline.zip` (FFMI.html + BACA-DULU.txt).
- Pembatasan ini di sisi browser: cukup untuk pengguna umum, bukan keamanan kuat.

## User Manual
Manual ada di dalam aplikasi (menu Panduan, juga dari layar login), Indonesia dan English. Isinya ada di konstanta `MAN` dan `CHANGELOG` dalam `index.html`.

## CHECKLIST SETIAP UPDATE (wajib)
1. Ubah aplikasi di `index.html` (jika sumbernya FFMI.html offline yang baru, terapkan ulang lapisan web).
2. Perbarui bagian terkait di `MAN` (id dan en) dan tambah entri di `CHANGELOG`.
3. Naikkan `APP_VER` dan `APP_DATE` di `index.html`, dan `VERSION` di `sw.js` (mis. `ffmi-1.3.1`).
4. Buat ulang `download/FFMI-offline.zip`: salin `index.html` menjadi `FFMI.html`, zip bersama `BACA-DULU.txt`.
5. Perbarui judul versi README ini, lalu commit dan push.

## Catatan
- Data terikat ke browser dan alamat/berkas yang dipakai. Data akun dari versi web sebelumnya tetap terbaca dan dimigrasi otomatis.
- Pindah perangkat lewat Backup lalu Restore (Premium). Ingatkan pengguna untuk Backup berkala.
