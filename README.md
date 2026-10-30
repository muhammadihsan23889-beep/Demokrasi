# Detektif Demokrasi: Misteri Santunlandia

Game edukasi Pendidikan Pancasila untuk SMA/SMK Kelas XI, bertema **Perilaku Demokratis pada Era Keterbukaan Informasi**.

## Isi paket

- `index.html` — seluruh HTML, CSS, JavaScript, materi, dan game dalam satu berkas.
- `README.md` — petunjuk pemasangan dan pengelolaan.

## Publikasi dengan GitHub Pages

1. Masuk ke [github.com](https://github.com) dan buat repository baru, misalnya `detektif-demokrasi`.
2. Unggah **`index.html` dan `README.md` ke folder utama (root)** repository, bukan ke dalam subfolder.
3. Buka **Settings → Pages**.
4. Pada **Build and deployment**, pilih **Deploy from a branch**.
5. Pilih branch **main** dan folder **/(root)**, lalu tekan **Save**.
6. Setelah GitHub selesai menerbitkan situs, buka `https://NAMA-PENGGUNA.github.io/detektif-demokrasi/` (ganti `NAMA-PENGGUNA` dengan username GitHub Anda). Publikasi bisa memerlukan beberapa menit.

## Mengubah materi atau soal

Buka `index.html` dengan VS Code atau editor teks, cari `const BANK_SOAL`, ubah pertanyaan, pilihan, jawaban, dan umpan balik, lalu commit perubahan ke repository. Jangan mengubah struktur data tanpa menyesuaikan logika game.

**Penting:** Lengkapi dan verifikasi placeholder data Indeks Demokrasi EIU dan 10 prinsip demokrasi Ahmad Sanusi berdasarkan infografis sumber sebelum digunakan sebagai materi resmi.

## Memainkan di Android

Buka tautan GitHub Pages menggunakan Chrome Android. Antarmuka dirancang responsif. Untuk penggunaan offline, simpan `index.html` ke perangkat dan buka sebagai file lokal pada browser yang mengizinkannya.

## Ranking dan penyimpanan

Skor dan kemajuan tersimpan secara lokal di browser menggunakan `localStorage` bila diizinkan. **GitHub Pages tidak otomatis menggabungkan ranking antarperangkat.** Ranking bersama memerlukan layanan backend/database (misalnya Firebase atau Supabase), aturan keamanan, serta perubahan JavaScript untuk mengirim dan mengambil hasil. Jangan menganggap skor dari browser sebagai data yang anti-manipulasi.

Untuk penggunaan bersama siswa, hindari memasukkan informasi pribadi yang tidak diperlukan. Pertimbangkan nama panggilan/kode peserta dan kelas alih-alih nama lengkap pada leaderboard publik.

## Troubleshooting

- **404:** Pastikan nama file persis `index.html`, terletak di root, dan pengaturan Pages menunjuk branch/folder yang benar.
- **Belum muncul:** Tunggu deployment pada tab **Actions** atau halaman **Settings → Pages**, lalu muat ulang.
- **Kemajuan hilang:** Periksa apakah browser memakai mode privat, data situs terhapus, atau domain berubah.
- **Ranking tidak sinkron:** Ini memang keterbatasan versi statis, bukan kesalahan GitHub Pages.

## Catatan pengujian

Berkas berasal dari game V3 yang tersedia pada percakapan ini. Publikasi dan pengujian menyeluruh pada berbagai perangkat belum dilakukan; uji setiap babak sebelum dipakai dalam pembelajaran atau kompetisi.
