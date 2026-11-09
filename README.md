# KeepOnLearn

**Tetap belajar, sinyal atau tidak.**

KeepOnLearn adalah aplikasi web progresif untuk latihan Matematika SMP kelas 7. Aplikasi ini menyesuaikan soal dengan penguasaan setiap siswa dan **tetap berjalan tanpa internet** setelah dibuka sekali.

**Coba langsung:** https://aryafajar200.github.io/KeepOnLearn/

Dibuat oleh Tim KuroRegist, Universitas Telkom, untuk ADIKARA 2026 (divisi Inovasi, sub Software). Mendukung SDG 4 (target 4.1) dan Asta Cita poin 4 dan 6.

## Masalah yang dijawab

Skor matematika Indonesia pada PISA 2022 adalah 366, turun 13 poin dari 2018. Sebagian SMP juga belum memiliki akses internet. Siswa dengan koneksi terbatas sulit mendapat latihan tambahan, dan guru sulit melihat topik mana yang perlu diulang. Rincian data dan sumbernya ada di proposal.

## Fitur

- **Kuis diagnostik** enam soal untuk mengukur penguasaan awal tiap topik.
- **Latihan adaptif** yang memilih soal dari topik dengan penguasaan terendah pada tingkat kesulitan yang sesuai.
- **Pengulangan terjadwal** untuk soal yang pernah salah (kotak Leitner).
- **Jalur kejar**: bila penguasaan suatu topik di bawah 40%, tersedia empat soal prasyarat setara SD akhir.
- **Pelajaran interaktif** langkah demi langkah (batang pecahan, timbangan persamaan, harga dan skala). Ini bukan video rekaman.
- **Mode guru**: impor berkas hasil siswa, lihat ringkasan kelas, topik terlemah, dan kelompok remedial.
- **Teks besar** dan **baca soal dengan suara** perangkat.
- **Mode offline** penuh setelah pemasangan pertama.

## Cara mencoba (2 menit)

1. Buka tautan di atas dengan Chrome atau peramban berbasis Chromium.
2. Masukkan nama panggilan, lalu pilih **Mulai diagnostik** dan jawab enam soal.
3. Perhatikan bagian **Jalur kejar** yang muncul untuk topik yang masih lemah.
4. Buka tab **Pelajaran** dan coba geser batang pecahan.
5. Buka tab **Guru**, pilih **Lihat dengan data contoh** untuk melihat ringkasan kelas dan kelompok remedial.
6. Untuk mencoba offline: tunggu tulisan "Siap dipakai tanpa sinyal", matikan internet, lalu muat ulang. Aplikasi tetap terbuka.

## Data dan privasi

- Aplikasi **tidak memiliki server dan tidak mengirim data apa pun**. Nama dan hasil belajar hanya tersimpan di peramban perangkat pengguna (IndexedDB).
- Data dari siswa ke guru berpindah **hanya lewat berkas** yang diserahkan siswa dan diimpor guru.
- Data di mode Guru berlabel **"data contoh"** adalah contoh tampilan, bukan siswa nyata.
- Untuk menghapus data di perangkatmu: tekan F12, tab Application, Storage, **Clear site data**.

## Batasan yang kami akui

- Soal hanya **Matematika SMP kelas 7** (30 soal) dan **12 soal prasyarat** setara SD akhir yang **belum divalidasi guru**. Belum ada paket SD lengkap, SMA, atau mata pelajaran lain.
- **Belum diuji pada siswa dan guru sungguhan.** Parameter algoritma adaptif belum dikalibrasi dengan data nyata.
- Pemasangan pertama membutuhkan koneksi internet satu kali.
- Baca soal dengan suara memakai suara bawaan perangkat; kualitas dan ketersediaan suara berbahasa Indonesia berbeda tiap perangkat dan belum diuji pada ponsel nyata.
- Data tidak dienkripsi dan hilang bila data peramban dihapus.

## Pengujian

- 22 uji unit untuk mesin adaptif dan bank soal (kunci jawaban soal hitungan diperiksa dengan hitungan independen).
- 82 pemeriksaan otomatis di peramban berbasis Chromium (alur dasar 40, fitur baru 42), termasuk mode offline, tanpa gulir horizontal, target sentuh minimal 44 piksel, dan fokus papan ketik.
- Seluruhnya lulus, dan rangkaian fitur baru stabil pada lima kali jalan berturut-turut. Pengujian belum mencakup beragam perangkat Android dan peramban selain Chromium.

## Teknologi

React 19, Vite, vite-plugin-pwa (Workbox), IndexedDB, dan Web Speech API.

Repositori ini hanya berisi **berkas hasil build** untuk hosting di GitHub Pages.

## Tim

Tim **KuroRegist**: Arya Fajar Pratama (ketua) dan Avatariani Purnama Devi.
