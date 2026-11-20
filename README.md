# QuizMate VINIX7 (versi aplikasi berfungsi)

Aplikasi kuis interaktif berbasis HTML + CSS + JavaScript murni (tanpa build tool, tanpa backend).

## Fitur
- **Login** dengan validasi email/kata sandi, "Ingat saya", sesi tersimpan.
- **Katalog**: pencarian, filter kategori & status, statistik, progres, leaderboard.
- **Kuis** (Modul 4, 15 soal): timer 25 menit (auto-submit), navigasi soal, tandai ragu-ragu, simpan otomatis, pintasan keyboard (A–D, ← →).
- **Konfirmasi** dengan matriks verifikasi jawaban.
- **Evaluasi**: skor otomatis, status lulus (passing grade 75), review & pembahasan dengan filter, ulangi kuis.
- **Search**, **Profil**, **Leaderboard (Coming Soon)**.
- Data tersimpan di `localStorage` browser.

## Struktur
```
index.html   css/app.css   js/data.js (data modul & soal)   js/app.js (logika & router)
```
Tambah soal/modul di `js/data.js`.

## Jalankan lokal
```bash
python3 -m http.server 8000   # buka http://localhost:8000
```

## Deploy ke GitHub Pages
```bash
git init && git add . && git commit -m "QuizMate VINIX7"
git branch -M main
git remote add origin https://github.com/USERNAME/quizmate-vinix7.git
git push -u origin main
```
Lalu **Settings → Pages → Source: GitHub Actions**.

Login demo: email apa pun yang valid (mis. `siti@email.com`) dan kata sandi minimal 6 karakter.
