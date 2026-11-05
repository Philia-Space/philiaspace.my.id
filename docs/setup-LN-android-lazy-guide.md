<!-- upstream: setupLnOnAndroid @ 2026-07-12 -->
# Setup Mining LN, Buku, dan sejenisnya di Android [Lazy Guide](https://lazyguidejp.github.io/jp-lazy-guide/setupLnOnAndroid/)

---

 Diunggah: 24 Agustus 2025 · Diperbarui: 5 November 2026 – `Yaaacha`

---

- Kamu bisa membaca light novel di HP Android lewat Firefox atau Edge Canary sambil scan kata pakai Yomitan.

---

## Unduh dan Pasang

- Unduh dan pasang file `.apk` [Ankiconnect Android](https://github.com/KamWithK/AnkiconnectAndroid/releases/latest)

- Pasang [Ankidroid](https://play.google.com/store/apps/details?id=com.ichi2.anki)

**Syarat:**

- [Yomitan di Android](setup-yomitan-android-lazy-guide.md) sudah terpasang

---

## Pengaturan Awal

1. Buka `AnkiConnect Android`, lalu nyalakan service-nya  
    - Buka Ankidroid dan biarkan tetap berjalan di latar belakang

2. Di Firefox atau Edge Canary, buka `Yomitan Settings` > `Profile`, lalu atur `Default` & `Editing` Profile ke `Android (Anime, LN & Manga)`  
    - Kalau kamu tidak memakai pengaturan Yomitan dari LazyGuide, cek [Info 2](setup-LN-android-lazy-guide.md/#info-2-text-replacement-pattern)

     ![Yomitan Profile Android](img/yomitan-profile-android.png){height=250 width=500}

3. Di Firefox atau Edge Canary, buka `https://app.yatsu.moe/`, lalu unggah file EPUB light novel kamu

4. Sekarang kamu bisa mining di HP dengan menekan kata untuk scan

     ![Yatsu Reader Android](img/ttu-android.png){height=150 width=300}

Sekarang kamu bisa membaca light novel di Android.

---

## Info Tambahan dan Tips

#### Info 1: Pengaturan Yatsu Reader dari LazyGuide

??? info "Pengaturan Yatsu Reader dari LazyGuide <small>(klik di sini)</small>"

    Pengaturan Yatsu Reader di Android yang dipakai LazyGuide:

    ![Yatsu Reader Settings Android](img/ttu-settings-android.png){height=500 width=1000}

#### Info 2: Text Replacement Pattern

??? info "Text Replacement Pattern <small>(klik di sini)</small>"

    Kalau tidak memakai pengaturan dari LazyGuide, kamu harus memasukkan pola ini secara manual supaya scan teks lebih akurat:

    1. Di `Yomitan settings`, nyalakan `Advanced` (letaknya di pojok kiri bawah, atau gulir ke bawah)
    2. Buka `Translation` > `Configure custom text replacement patterns...`
    3. Salin dan tempel isi [tautan ini](https://pastebin.com/er57E9Hw)

#### Info 3: Android Yomitan Local Audio

??? info "Android Yomitan Local Audio <small>(klik di sini)</small>"

    **Syarat:**

    - Kamu sudah mengikuti [PC Yomitan Local Audio](setup-yomitan-pc-lazy-guide.md/#info-1-yomitan-local-audio)
    - [Ankiconnect Android](https://github.com/KamWithK/AnkiconnectAndroid/releases/latest) sudah terpasang
    - Info lengkap dan pembaruannya ada di [sini](https://github.com/Aquafina-water-bottle/AnkiconnectAndroid/tree/local_audio#additional-instructions-local-audio)
    - Setup ini butuh ruang penyimpanan **3GB+**

    ---
    1. Di Anki PC, klik `Tools` > `Local Audio Server` > `Generate Android database`  
         - Prosesnya 30+ menit. Selama itu Anki tidak bisa dipakai, tapi kamu masih bisa mining

    2. Di Anki PC, tekan ++ctrl+shift+a++ (Windows) / ++cmd+shift+a++ (MacOS) atau klik `Tools` > `Add-ons`, pilih `Local Audio Server for Yomitan`, lalu klik `View Files`  
         - Di sana ada file bernama `android` atau `android.db`

    3. Di Android, buka `AnkiConnect Android` > `Settings` > `Print Local Audio Directory`  
         - Aplikasi akan menampilkan path dan membuat foldernya

    4. Buka lokasi dari langkah 3, biasanya `Android/data/com.kamwithk.ankiconnectandroid/files/`  
         - Tempel file `android` dari PC (langkah 2) ke folder `files`  
         - Hasilnya harus: `Android/data/com.kamwithk.ankiconnectandroid/files/android.db`  
         - Kalau hanya punya HP Android, pakai file manager [MiXplorer](https://forum.xda-developers.com/t/app-2-2-mixplorer-v6-x-released-fully-featured-file-manager.1523691/#post-23109280)  
         - Pilih `Copy` dari folder unduhan, jangan `Cut`, supaya bisa `Paste`.

    5. Pakai profil `Android (Anime, LN & Manga)` dari `local-audio-yomitan-settings` LazyGuide  
         - Kalau tidak memakai profil itu, buka `Yomitan settings` > `Audio` > `Configure audio playback sources...` > `Add` > `Custom URL (JSON)`  
         - Tempel: `http://localhost:8765/localaudio/get/?term={term}&reading={reading}`  
           dan pastikan sumber ini ada di paling atas

    6. Cek apakah semua sumber audio muncul  
         - Kalau tidak jalan, pastikan `Start Service` di AnkiConnect Android aktif  
         - Matikan optimasi baterai (*battery optimization*) untuk AnkiConnect Android, Ankidroid, dan Firefox/Edge Canary

          ![Yomitan Local Audio Check](img/yomitan-local-audio-check.gif){height=250 width=500}

        Selesai!

---

## Pertanyaan Umum

#### Pertanyaan 1: Bagaimana cara memakai Monolingual Setup di Android?

??? question "Bagaimana cara memakai Monolingual Setup di Android? <small>(klik di sini)</small>"

    1. Buka `Yomitan settings` > `Dictionary`, lalu nyalakan `all`

        ![Dictionary Toggle](img/dictionary-toggle.png){height=250 width=500}
