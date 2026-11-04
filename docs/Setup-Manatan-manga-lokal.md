---
title: Manga Lokal
description: Struktur folder manga lokal yang didukung untuk Manatan.
---

# Manga Lokal

Manatan dapat membaca manga yang tersimpan secara lokal di perangkat, dari folder gambar, file arsip, atau file EPUB.

## Atur folder manga lokal

1. Buka **Settings** > **Browse**.
2. Atur **Local Manga source location** menuju folder penyimpanan manga lokalmu.
3. Buka **Browse** > **Source** > **Local source**.
4. Pilih serial yang ingin dibaca.

Jika Kamu menambahkan bab baru di kemudian hari, segarkan daftar bab.

---
## Struktur folder yang didukung

Di dalam folder manga lokal kamu, Manatan mendukung dua cara:

- satu folder untuk setiap serial, berisi folder bab, file arsip, atau file EPUB
- satu file `.epub`, `.zip`, `.cbz`, `.rar`, atau `.cbr` yang langsung ditaruh di folder utama

### File tunggal di folder utama

Cocok untuk oneshot atau satu volume utuh. Taruh filenya langsung di folder manga lokal.

```text
📁 [Folder Manga lokal]
├─ 📦 Look Back.cbz
├─ 📦 Oneshot Saya.zip
├─ 📦 Cerita Pendek.cbr
├─ 📦 Bab Bonus.rar
└─ 📘 Volume Full Color.epub
```

Setiap file muncul sebagai manga sendiri, dengan judul dari nama filenya (`Look Back.cbz` jadi *Look Back*). Kurang cocok untuk serial yang masih berjalan, karena tiap file akan muncul sebagai manga terpisah, bukan dikelompokkan.

### Folder serial berisi folder bab (direkomendasikan)

```text
📁 [Folder Manga lokal]
├─ 📁 Judul Serial
│   ├─ 🖼️ cover.jpg
│   ├─ 📁 001
│   │   ├─ 🖼️ 001.jpg
│   │   └─ 🖼️ 002.jpg
│   └─ 📁 002
│       ├─ 🖼️ 001.jpg
│       └─ 🖼️ 002.jpg
```

### Folder serial berisi file arsip
```text
📁 [Folder Manga lokal]
├─ 📁 Judul Serial
│   ├─ 📦 001.cbz
│   ├─ 📦 002.cbz
│   ├─ 📦 003.cbr
│   └─ 📦 004.rar
```

### Folder serial berisi file EPUB

Satu EPUB untuk tiap volume atau bab.

```text
📁 [Folder Manga lokal]
├─ 📁 Judul Serial
│   ├─ 📘 Volume 01.epub
│   └─ 📘 Volume 02.epub
```

Format yang didukung: folder gambar, `.zip`/`.cbz`, `.rar`/`.cbr`, dan `.epub`. Halaman gambar bisa berformat `.jpg`, `.jpeg`, `.jfif`, `.png`, `.webp`, `.gif`, `.bmp`, `.jxl`, atau `.avif`.

### Pilih yang mana?

- **File tunggal di folder utama**: untuk oneshot atau satu volume utuh, kalau mau paling cepat (taruh file lalu refresh) dan tidak butuh `cover.jpg` sendiri
- **Folder serial**: kalau ada beberapa bab/volume yang harus jadi satu judul, mau pakai `cover.jpg` atau `ComicInfo.xml`, atau babnya masih akan bertambah
    - Pakai **folder gambar** kalau mau mengecek atau mengganti halaman satu per satu
    - Pakai **file arsip** kalau mau file lebih sedikit dan sinkronisasi lebih rapi
    - Pakai **EPUB** kalau manga-nya memang sudah berbentuk EPUB. Untuk novel EPUB yang isinya teks, lebih baik pakai [Novel (EPUB)](Setup-Manatan-novels.md)

---
## Masalah Umum

#### Masalah 1: Serial saya tidak muncul

???+ note question "Serial saya tidak muncul"

    1. Pastikan jalur (path) folder sudah benar.
    2. Pastikan file di folder utama berformat `.epub`, `.zip`, `.cbz`, `.rar`, atau `.cbr`, atau folder/file bab berada di dalam folder serial.
    3. Segarkan daftar.

#### Masalah 2: Bab berada dalam urutan yang salah

???+ note question "Bab berada dalam urutan yang salah"

    Gunakan penamaan dengan awalan nol seperti `001`, `002`, `010`. Untuk file arsip, urutan halaman diambil dari nama file gambar di dalamnya. Untuk EPUB, urutannya mengikuti urutan di dalam EPUB.

#### Masalah 3: Galeri Android menampilkan gambar manga

???+ note question "Galeri Android menampilkan gambar manga"

    Buat file kosong bernama `.nomedia` di dalam folder lokal.
	