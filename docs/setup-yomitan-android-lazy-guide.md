<!-- upstream: setupYomitanOnAndroid @ 2026-07-12 -->
# Setup Yomitan di Android [LazyGuide](https://lazyguidejp.github.io/jp-lazy-guide/setupYomitanOnAndroid/)

---

 Diunggah: 24 Agustus 2025 · Diperbarui: 5 November 2026 – `Yaaacha`

---

- Yomitan adalah kamus hover untuk bahasa Jepang
- Dipakai untuk mining kata ke Anki
- Yomitan [Light](img/yomitan-light.png) | [Dark](img/yomitan-dark.png) Mode ([CSS](https://pastebin.com/T9EkQQwm))

---

## Unduh dan Pasang

- Pasang [Firefox](https://play.google.com/store/apps/details?id=org.mozilla.firefox) atau [Edge Canary](https://play.google.com/store/apps/details?id=com.microsoft.emmx.canary)

- Unduh dari [sini](https://drive.google.com/drive/folders/1DHJ18Lk2_tVYWJ1Adhe8XByuyFBGuTr_?usp=sharing):
    - `Font`
    - `yomitan dictionary`
    - `lazyGuide-yomitan-settings` (unduh keduanya)
        - Firefox: `yomitan settings` [di sini](https://drive.google.com/drive/folders/1D_O7HgX4xMBOQcl2tLoeAQ7KUtPqyUnU?usp=sharing)
    - Tambahan kamus [JIDict](https://github.com/philiaspaceai/JIDict-yomitan#pemasangan) (Jepang-Indonesia)

- Setelah diunduh:
    - Ekstrak `Font.7z` dan `yomitan dictionary.7z` (password: `lazyguide`)
    - `yomitan dictionary.7z` cukup diekstrak sekali, **jangan ekstrak kamus di dalamnya**.

---

## Pengaturan Awal

Pasang Yomitan sesuai browser yang kamu pilih:

=== "Firefox"

    1. Pasang [Yomitan dari Firefox Add-ons](https://addons.mozilla.org/en-US/android/addon/yomitan/)

    2. Buka `Settings` > `Extensions`, tekan `Yomitan Popup Dictionary`, lalu tekan `Settings` (ikon roda gigi)

    3. Di `Welcome Page`, nyalakan `Enable optional permissions`

         ![Enable optional permissions](img/enable-optional-permissions.png){height=200 width=400}

=== "Edge Canary"

    1. Buka `Menu` > `Settings` > `About Microsoft Edge` > `Privacy and Terms`, lalu tekan `Edge Canary build number` 7 kali  
        - `Developer Options` akan aktif

         ![Edge Canary Build Number](img/edge-canary-build-number.png){height=200 width=400}

    2. Kembali ke `Settings` > `Developer Options` > `Extension install by id`, lalu tempel ID ini:

        ```bash
        idelnfbbmikgfiejhgmddlbkfgiifnnn
        ```

    3. Tekan `Add` untuk memasang Yomitan, lalu tunggu sampai unduhannya selesai  
        - `Welcome Page` akan muncul otomatis. Bisa juga dibuka lewat `Settings` > `Extensions` > `Yomitan Popup Dictionary` > `Settings` (ikon roda gigi)

    4. Di `Welcome Page`, nyalakan `Enable optional permissions`

         ![Enable optional permissions](img/enable-optional-permissions.png){height=200 width=400}

Setelah itu, langkahnya sama untuk kedua browser:

1. Buka `Settings Page`, atau buka `Settings` > `Extensions` > `Yomitan Popup Dictionary` > `Settings` (ikon roda gigi)

2. Buka `Dictionary` > `Configure installed and enabled dictionaries...` > `Import`
     - Impor semua kamus dari folder `yomitan dictionary` (semuanya bisa dipilih sekaligus)
     - Nyalakan `JIDict` dan taruh di prioritas #1 (paling atas)

     ![Dictionary Import](img/yomitan-dictionary-import.png){height=250 width=500}

3. Gulir ke bawah ke `Backup`, tekan `Import Settings`, lalu pilih `lazyGuide-yomitan-settings` (file dari [sini](setup-yomitan-android-lazy-guide.md/#unduh-dan-pasang))
     - Pilih salah satu:
         - `lazyGuide-local-audio-yomitan-settings` (pasang juga [Yomitan Local Audio](setup-yomitan-android-lazy-guide.md/#info-1-android-yomitan-local-audio) kalau memakai yang ini)
         - `lazyGuide-non-local-audio-yomitan-settings`

         ![Yomitan Import Settings](img/yomitan-import-settings.png){align=left height=300 width=600}

4. Pilih profil `Android (Anime, LN & Manga)` sebagai `Active Profile`

     ![Yomitan Profile](img/yomitan-profiles.jpg){align=left height=300 width=600}

Setup Yomitan selesai.

<small>Kalau ada masalah, cek [FAQs](setup-yomitan-android-lazy-guide.md/#pertanyaan-umum)</small>

---

## Info Tambahan dan Tips

#### Info 1: Android Yomitan Local Audio

??? info "Android Yomitan Local Audio <small>(klik di sini)</small>"

    Syarat:
    
    - Kamu sudah mengikuti [PC Yomitan Local Audio](setup-yomitan-pc-lazy-guide.md/#info-1-yomitan-local-audio)
    - [Ankiconnect Android](https://github.com/KamWithK/AnkiconnectAndroid/releases/latest) sudah terpasang
    - Info lengkap dan pembaruannya ada di [sumber utama](https://github.com/Aquafina-water-bottle/AnkiconnectAndroid/tree/local_audio#additional-instructions-local-audio)
    - Setup ini butuh ruang penyimpanan **3GB+**

    ---
    1. Di Anki PC, klik `Tools` > `Local Audio Server` > `Generate Android database`  
         - Prosesnya 30+ menit. Selama itu Anki tidak bisa dipakai, tapi kamu masih bisa mining
    
    2. Di Anki PC, tekan ++ctrl+shift+a++ (Windows) / ++cmd+shift+a++ (MacOS) atau klik `Tools` > `Add-ons`, pilih `Local Audio Server for Yomitan`, lalu klik `View Files`  
         - Di sana ada file `android` atau `android.db`

    3. Di Android, buka `AnkiConnect Android` > `Settings` > `Print Local Audio Directory`  
         - Aplikasi akan menampilkan path dan membuat foldernya

    4. Buka lokasi dari langkah 3, biasanya `Android/data/com.kamwithk.ankiconnectandroid/files/`  
         - Tempel file `android` dari PC (langkah 2) ke folder `files`  
         - Hasilnya harus: `Android/data/com.kamwithk.ankiconnectandroid/files/android.db`

    5. Pakai profil `Android (Anime, LN & Manga)` dari `local-audio-yomitan-settings` LazyGuide  
         - Kalau tidak memakai profil itu, buka `Yomitan settings` > `Audio` > `Configure audio playback sources...` > `Add` > `Custom URL (JSON)`  
         - Tempel:  
           `http://localhost:8765/localaudio/get/?sources=jpod,jpod_alternate,nhk16,forvo&term={term}&reading={reading}`  
           dan pastikan sumber ini ada di paling atas

    6. Cek apakah semua sumber audio muncul  
         - Kalau tidak jalan, pastikan `Start Service` di AnkiConnect Android aktif  
         - Matikan optimasi baterai (*battery optimization*) untuk AnkiConnect Android, Ankidroid, dan Firefox/Edge Canary

          ![Yomitan Local Audio Check](img/yomitan-local-audio-check.gif){height=250 width=500}

          Selesai!

#### Info 2: Yomitan Light dan Dark Mode

??? info "Yomitan Light dan Dark Mode <small>(klik di sini)</small>"

    Untuk mengganti tema Yomitan, buka `Yomitan settings` > `Appearance` > `Theme`

    ![Yomitan Theme](img/yomitan-theme.png){height=300 width=600}

---

## Pertanyaan Umum

#### Pertanyaan 1: Boleh menambah kamus Yomitan sendiri?

??? question "Bolehkah menambah, menghapus, atau mengubah kamus Yomitan? <small>(klik di sini)</small>"

    - Silakan. Sebagian besar kamus berformat Yomitan bisa dipakai. Cara memasangnya ada di langkah 6 bagian [Setup Yomitan PC](setup-yomitan-pc-lazy-guide.md/#setup)

    - Kamu juga bisa mengubahnya di `Yomitan settings` > `Anki` > `Configure Anki card format...` > `MainDefinition`, lalu pilih `single-glossary-YANG-KAMU-MAU` dari dropdown

    - Kalau mengganti `MainDefinition`, kamu harus mengubahnya di setiap `Profile`

#### Pertanyaan 2: Cari kamus lainnya di mana?

??? question "Cari kamus lainnya di mana? <small>(klik di sini)</small>"

    - Koleksi kamus lain ada di [koleksi Shoui](https://learnjapanese.link/dictionaries) dari TMW atau [koleksi Marv](https://drive.google.com/drive/folders/1xURpMJN7HTtSLuVs9ZtIbE7MDRCdoU29) dari Yomitan

#### Pertanyaan 3: Rekomendasi Kamus Frequency?

??? question "Rekomendasi kamus frekuensi? <small>(klik di sini)</small>"

    - JPDB
        - Daftar frekuensi dari [jpdb.io](https://jpdb.io), situs yang menganalisis banyak *light novel*, *visual novel*, anime, dan *J-drama*. Jadi, daftar ini menunjukkan seberapa sering sebuah kata muncul di media fiksi berbahasa Jepang.
    - CC100
        - Daftar frekuensi dari korpus internet Jepang. Kata formal akan terlihat lebih umum di daftar ini.  
        - Contoh: 審議会 (*council*) ada di peringkat ke-9733 di CC100, tetapi ke-58730 di JPDB.

#### Pertanyaan 4: Apa yang dimaksud dengan "kata umum"?

??? question "Apa yang dimaksud dengan “kata umum”?  <small>(klik di sini)</small>"

    - **Sangat umum:** 1–10.000
    - **Umum:** 10.001–20.000
    - **Cukup umum:** 20.001–30.000
    - **Agak jarang:** 30.001–40.000
    - **Jarang:** 40.001–50.000
    - **Sangat jarang:** 50.001–80.000
    - **Tingkat yang mungkin tidak dikenal penutur asli:** 80.000+

#### Pertanyaan 5: Kapan kamus diperbarui? Harus memperbarui sendiri?

??? question "Kapan kamusnya diperbarui? Perlu memperbarui sendiri? <small>(klik di sini)</small>"

    - Kamus di panduan ini jarang diperbarui. Tidak perlu buru-buru ke versi terbaru karena isinya jarang berubah.  
      - Tujuannya stabilitas jangka panjang tanpa repot memperbarui.  
      - Kalau kamu mau versi yang paling baru, kamusnya bisa diperbarui sendiri.

#### Pertanyaan 6: Bagaimana cara memakai sentence card?

??? question "Bagaimana cara memakai sentence card? <small>(klik di sini)</small>"

    Buka `Yomitan settings` > `Anki` > `configure Anki flashcard...`

    ![Sentence Card Instruction 1](img/yomitan-anki-active-profile.jpg){height=300 width=600}
    
    Di `Expression`, gulir ke bawah dan cari `IsSentenceCard`. Ubah nilainya jadi `1`, lalu tutup.

    ![Sentence Card Instruction 2](img/yomitan-sentence-card.jpg){height=300 width=600}

    Terapkan ini di semua profil. Pastikan konfigurasi `Monolingual`, `Bilingual`, `Android (Anime, LN & Manga)`, dan `Android (VN)` sudah diubah.

    ![Yomitan Profile](img/yomitan-profiles.jpg){align=left height=300 width=600}
