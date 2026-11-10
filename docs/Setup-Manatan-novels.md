---
title: Novel (EPUB)
description: Impor dan baca novel EPUB di Manatan.
---

# Novel (EPUB)

Impor file EPUB, PDF, atau TXT, lalu baca dengan kamus popup.

---

## Impor buku

1. Buka menu `Novels`.
2. Tekan ikon tiga titik di kanan atas, lalu pilih `Import EPUB, PDF or TXT`.
3. Pilih file bukunya. Setelah muncul di daftar, tekan sampulnya untuk mulai membaca.
   > **NB:** Manatan hanya menerima EPUB, PDF, dan TXT. File lain seperti `.azw3` atau `.mobi` perlu dikonversi dulu ke EPUB dengan aplikasi lain, misalnya [Calibre](https://calibre-ebook.com/). Pakai file yang tidak terenkripsi (tanpa DRM).

![Menu impor buku di Novels Manatan](img/manatan-novel-import.jpg){height=500 width=500}

---

## Audiobook

Manatan bisa memutar audiobook bersamaan dengan bukunya. Kalimat yang sedang dibacakan disorot, dan halaman ikut berpindah mengikuti suara.

Fitur ini hanya ada di aplikasi Manatan versi sekarang (dicoba di versi 6.3.14). Versi lama yang dibuka lewat browser (Web UI) tidak punya fitur ini.

1. Buka bukunya, lalu munculkan bilah menu di bagian atas layar dan pilih `Audiobook`.
2. Pilih file audionya. Format yang diterima: MP3, M4B, M4A, Ogg, Opus, FLAC, dan WAV.
3. Supaya suara bisa mengikuti teks, Manatan butuh data waktu tiap kalimat. Ada dua cara:
    - Impor file subtitle audiobook-nya (SRT, VTT, atau LRC) kalau punya.
    - Kalau tidak punya, biarkan Manatan membuat transkripnya sendiri dari audio. Prosesnya berjalan di perangkatmu dan bisa lama untuk audiobook yang panjang.
4. Setelah teks dan suara cocok, bilah putar muncul di bagian bawah layar.
   > **NB:** Kalau muncul pesan `No text matched`, periksa apakah audio, subtitle, dan bukunya berasal dari edisi yang sama.

Tombol di bilah putar, dari kiri ke kanan:

| Tombol | Fungsi |
|---|---|
| Mundur | Kalimat sebelumnya |
| Putar/jeda | Memutar atau menjeda audiobook |
| Ulang | Mengulang kalimat yang sedang dibacakan |
| Maju | Kalimat berikutnya |
| Garis waktu | Pindah ke bagian lain audiobook |
| Headphone | Pengaturan audiobook, misalnya kecepatan putar dan warna sorotan |

Selain audiobook, ikon speaker di bilah atas pembaca tetap bisa dipakai untuk text-to-speech (dibacakan suara buatan).

Pilihan lain untuk membaca sambil mendengarkan audiobook: [Yatsu Reader dengan Yatsu Whispersync](setup-LN-pc-lazy-guide.md#info-3-audiobook-dengan-yatsu-whispersync) di PC, [Hoshi Reader](Setup-Hoshi-Reader.md#info-2-audiobook) di Android, atau [Hoshi Reader](Setup-Hoshi-Reader-iOS.md#audiobook-sasayaki) di iPhone dan iPad.

---

## Membaca

=== "Halaman Buku"
	![Halaman novel di pembaca Manatan](img/manatan-novel-reader.jpg){height=500 width=500}
=== "Pengaturan"
	![Pengaturan pembaca novel di Manatan](img/manatan-novel-settings.jpg){height=500 width=500}

- Klik atau ketuk bagian atas layar untuk memunculkan bilah menu. Pengaturan ada di ikon roda gigi `Novel settings` > tab `Novel`.
- Untuk mencari arti kata, arahkan kursor atau ketuk kata tersebut sampai popup kamus muncul.
- Kalau arti kata tidak muncul, pastikan kamus sudah diimpor dan popup untuk `Novel` sudah dinyalakan. Lihat [cara impor kamus](Setup-Manatan.md#kamus).
- Pastikan teksnya bisa dipilih. Kata di halaman yang isinya hanya gambar tidak bisa dicari langsung di kamus.

??? info "Isi bilah menu dan pengaturan pembaca <small>(klik di sini)</small>"

    Ikon di bilah atas, dari kiri ke kanan:

    | Ikon | Fungsi |
    |---|---|
    | Speaker | Text-to-speech (dibacakan suara buatan) |
    | Kaca pembesar | Cari kata di dalam buku |
    | Grafik | Statistik membaca |
    | Gambar | Galeri gambar di dalam buku |
    | Tanda kutip | Daftar highlight |
    | Daftar | Daftar isi |
    | Kotak | Layar penuh |
    | Roda gigi | Pengaturan |

    Pengaturan yang paling sering diubah di tab `Novel`:

    | Pengaturan | Isi |
    |---|---|
    | Theme | Warna latar: putih, terang, sepia, gelap, hitam |
    | Mode | `Paged` (per halaman) atau `Continuous` (digulir) |
    | Direction | `Vertical RTL` untuk teks tegak seperti buku Jepang, `Horizontal` untuk teks mendatar |
    | Font size, Line height | Ukuran huruf dan jarak baris |
    | Primary font | Jenis huruf. Beberapa perlu diunduh dulu |
    | Show furigana | Tampilkan atau sembunyikan furigana |
    | Reader status display | Tampilkan judul, jumlah huruf, dan persentase bacaan |

---

## Sinkronisasi antar perangkat (opsional)

Sinkronisasi tidak wajib. Kalau diaktifkan, progres membaca tetap sama di semua perangkatmu.

Manatan mengutamakan penyimpanan lokal (*local-first*), jadi tetap bisa dipakai secara luring kalau sinkronisasi dimatikan.

Sumber: [Novels (EPUB)](https://manatan.com/docs/guides/novels)
