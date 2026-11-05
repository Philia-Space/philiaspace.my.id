<!-- upstream: setupMangaOnAndroid @ 2026-07-12 -->
# Setup: Manga di Android
---

 Diunggah: 24 Agustus 2025 · Diperbarui: 5 November 2026 – `Yaaacha`

---

- Kamu bisa membaca manga di HP Android lewat Firefox atau Edge Canary sambil scan kata pakai Yomitan.
- Fitur screenshot manga otomatis juga tetap bisa dipakai di Android.

---

## Unduh dan Pasang

- Unduh dan pasang file `.apk` [Ankiconnect Android](https://github.com/KamWithK/AnkiconnectAndroid/releases/latest/) dari bagian `Assets`

- Pasang [Ankidroid](https://play.google.com/store/apps/details?id=com.ichi2.anki)

**Syarat:**

- [Yomitan di Android](setup-yomitan-android-lazy-guide.md) sudah terpasang
- Manga yang sudah diproses dari [Setup Mining Mokuro Manga](setup-manga-pc-lazy-guide.md/#setup-mining-mokuro-manga)
- Aplikasi kompres file seperti [7z](https://www.7-zip.org/)

---

## Pengaturan Awal

1. Di PC, kompres folder manga kamu (yang berisi folder `img` atau file `.png`) jadi format `.zip` (**bukan** `.7z`)  
    - Caranya: klik kanan folder > `7-Zip` > `Compress...` > `Archive Format: .zip` > `OK`

2. Pindahkan manga yang sudah diproses ke HP Android  
    - Semua file: file manga `.zip` hasil kompres, folder `_ocr`, dan file `.mokuro`

3. Buka `Ankiconnect Android` > `Settings` > `CORS Host`, lalu isi dengan `https://reader.mokuro.app`

     ![CORS Host](img/cors-host.png){height=200 width=400}

4. Tekan `Start the Service` di `AnkiConnect Android` dan pastikan AnkiDroid juga terbuka

5. Di Edge Canary, buka [Mokuro Reader](https://reader.mokuro.app/), tekan ikon `Upload` (kanan atas), lalu pilih `choose files` (**bukan** `choose directory`)  
    - Pilih file `.html`, `.mokuro`, dan `.zip` dari manga (hasil langkah 2)

     ![Mokuro Android Upload](img/mokuro-upload-android.png){height=150 width=300}

    ??? examplecode "Struktur Folder <small>(klik di sini)</small>"
        
        ```
        ├── Folder Manga
        │   ├── _ocr folder
        │   ├── .html
        │   ├── .mokuro
        │   └── .zip
        │   |    └── file gambar manga (.jpg/.png)
        ```

6. Di kanan atas, buka `settings` > `Profile` > `Select a File`, pilih file [Mokuro Profile](https://drive.google.com/drive/folders/17EzQL9ONQ3MVsCJwC7ejmL0317EwdR--?usp=sharing), tekan `Import Profiles`, lalu pilih `Mobile Profile`  
    - Kamu juga bisa membuat profil sendiri, asalkan bagian `Anki Connect` sudah diatur lengkap.

7. Untuk mining, tekan lama sebuah kata untuk scan, lalu tambahkan kata itu lewat Yomitan  
    - Untuk screenshot, ketuk dua kali atau tekan lama di dalam `text border` (bawaannya tidak terlihat)

     ![Mokuro Settings](img/mokuro-yomitan.png){height=400 width=800}

8. Sekarang kamu bisa mining dan screenshot manga di Android dengan mudah.

Setup mining manga di Android sudah selesai. 

<small>Kalau ada masalah, cek [FAQs](setup-manga-android-lazy-guide.md/#pertanyaan-umum)</small>

---

## Info Tambahan dan Tips

#### Info 1: Android Mining Demo

??? info "Android Mining Demo <small>(klik di sini)</small>"

    - Demo mining dengan screenshot manga
    - Videonya sudah agak lama, tapi masih menunjukkan fungsi dasarnya
    - Untuk screenshot, ketuk dua kali atau tekan lama di dalam `text border`

    ![Android Manga Mining](img/android-manga-mining.gif){height=200 width=400}

---

## Pertanyaan Umum

#### Pertanyaan 1: Bagaimana cara memakai Monolingual Setup di Android?

??? question "Bagaimana cara memakai Monolingual Setup di Android? <small>(klik di sini)</small>"

    1. Buka `Yomitan settings` > `Dictionary`, lalu nyalakan `all`

        ![Dictionary Toggle](img/dictionary-toggle.png){height=250 width=500}
