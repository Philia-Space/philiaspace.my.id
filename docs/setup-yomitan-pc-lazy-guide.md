# Setup Yomitan di PC [LazyGuide](https://lazyguidejp.github.io/jp-lazy-guide/setupYomitanOnPC/)

---

 Diunggah: 1 Agustus 2025 · Diperbarui: 5 November 2026 – `Yaaacha`

---

- Yomitan adalah kamus _pop-up_ untuk berbagai bahasa
- Dipakai untuk mining ke Anki
- Setup di tutorial ini memakai note type [Lapis](https://github.com/donkuri/lapis)
- Tampilan Yomitan: [Light](img/yomitan-light.png) | [Dark](img/yomitan-dark.png) ([CSS](https://pastebin.com/T9EkQQwm))

---

## Unduh dan Pasang

- Pasang [Yomitan untuk Chrome/Edge](https://chrome.google.com/webstore/detail/yomitan/likgccmbimhjbgkjambclfkhldnlhbnn) atau [Yomitan untuk Firefox](https://addons.mozilla.org/en-US/firefox/addon/yomitan/)

- Unduh file berikut dari [sini](https://drive.google.com/drive/folders/1DHJ18Lk2_tVYWJ1Adhe8XByuyFBGuTr_?usp=sharing):
    - `Font`
    - `kamus yomitan`
    - `lazyGuide-yomitan-settings` (unduh keduanya)
        - Firefox/Brave: unduh `yomitan settings` [di sini](https://drive.google.com/drive/folders/1D_O7HgX4xMBOQcl2tLoeAQ7KUtPqyUnU?usp=sharing)
    - Kamus tambahan [JIDict](https://github.com/philiaspaceai/JIDict-yomitan#pemasangan) (Jepang-Indonesia)
- Setelah diunduh:
    - Ekstrak `Font.7z` dan `yomitan dictionary.7z` (password: `lazyguide`)
    - `yomitan dictionary.7z` cukup diekstrak sekali. **Jangan ekstrak file kamus di dalamnya**

---

## Setup

1. Gulir ke bawah di halaman awal Yomitan, buka `Permissions page`, lalu aktifkan `clipboardRead` dan `nativeMessaging`

	???+ note "Klik tombol `Permission Page` di halaman izin Yomitan"
		![Yomitan Permission Page](img/pencet-tuh.jpg){height=250 width=500}
		
		<small>Klik tombol `Permission Page` di halaman izin Yomitan.</small>

	???+ note "Beri izin Yomitan"
		![Yomitan Permission Page](img/yomitan-permission.jpg){height=250 width=500}
		
		<small>Aktifkan `clipboardRead` dan `nativeMessaging` di bagian bawah.</small>

2. Buka `chrome://extensions`, `edge://extensions`, atau `about:addons` (Firefox), lalu buka pengaturan ekstensi Yomitan

3. Pastikan:
    - Chrome/Edge: aktifkan `Allow access to file URLs`
    - Firefox: aktifkan `Access your data for all websites`
    === "Chrome/Edge"
        ![Chrome/Edge URL Access](img/chromium-url-acces.jpg){height=150 width=300}
    === "Firefox"
        ![Firefox Yomitan Access to all websites](img/firefox-url-access.png){height=300 width=600}

4. Pasang font dengan membuka file-filenya di folder `Font`
   
    ![Yomitan Font](img/fonts.png){height=150 width=300}

5. Buka halaman pengaturan Yomitan (klik ikon ekstensi, lalu klik ikon gir)

    ![Yomitan Cog](img/yomitan-cog.jpg){height=50 width=100}

6. Buka `Dictionaries` > `Configure installed and enabled dictionaries...` > `Import`
    - Impor semua kamus dari folder `yomitan dictionary` (bisa dipilih sekaligus)
    - Aktifkan semua kamus
    - Taruh `JIDict`, `Jitendex`, atau kamus lain yang kamu mau di urutan paling atas (priority #1)
    ![Dictionary Import](img/yomitan-dictionary-import.png){height=250 width=500}

7. Gulir ke bawah ke bagian `Backup` > `Import Settings`, lalu pilih `lazyGuide-yomitan-settings` (yang sudah diunduh dari [sini](setup-yomitan-pc-lazy-guide.md/#unduh-dan-pasang))
    - Pilih salah satu:
        - `lazyGuide-local-audio-yomitan-settings` (butuh: [Yomitan Local Audio](setup-yomitan-pc-lazy-guide.md/#info-1-yomitan-local-audio))
        - `lazyGuide-non-local-audio-yomitan-settings`

        ![Yomitan Import Settings](img/yomitan-import-settings.png){align=left height=300 width=600}

8. Atur profil aktif
    - Pilih `Monolingual` sebagai `active profile`. Kamu juga bisa menahan ++alt++ (Windows) atau ++opt++ (MacOS) sambil mengarahkan kursor ke kata untuk beralih ke `Monolingual`
        ![Yomitan Profile](img/yomitan-profiles.jpg){height=300 width=600}

    - Buka pengaturan `Anki`, lalu pilih `Configure Anki flashcards...`
        ![Yomitan Active Profile](img/yomitan-anki-active-profile.jpg){height=300 width=600}
    - Ganti isi `MainDefinition` jadi `{single-glossary-jidict-v103}`
        - Angka di belakangnya mengikuti versi JIDict yang terpasang, jadi pilih saja `single-glossary-jidict-...` yang muncul di dropdown

        ![Yomitan Active Profile JIDict](img/yomitan-anki-active-profile-jidict.jpg){height=300 width=600}

    - Ulangi langkah 8 ini untuk profil `Bilingual`

9. Sekarang kamu sudah bisa mencari kata dengan mengarahkan kursor ke teks!
    - Untuk mengganti tombol pintasannya, buka `Yomitan settings` > `Scanning` > `Scan modifier key`

    === "Windows"
        ![Yomitan Scan Key](img/yomitan-scan-key.png){align=left height=300 width=600}
    === "MacOS"
        ![Yomitan Scan Key](img/yomitan-scan-key.jpg){align=left height=300 width=600}


Setup Yomitan di PC sudah selesai! Mau lanjut ke panduan Setup Mining Anime?

[Lanjut ke Setup Mining Anime di PC](setup-anime-pc-lazy-guide.md){ .md-button .md-button }

<small>Kalau ada masalah, cek bagian [Pertanyaan Umum](setup-yomitan-pc-lazy-guide.md/#pertanyaan-umum)</small>

---

## Info Tambahan dan Tips

#### Info 1: Yomitan Local Audio

??? info "Yomitan Local Audio <small>(klik di sini)</small>"

    - Cek [sumber aslinya](https://github.com/yomidevs/local-audio-yomichan) untuk info dan pembaruan terbaru
    - Prosesnya bisa makan waktu sekitar satu jam dan butuh Anki versi 2.1.50+
    - Versi Android [juga ada](https://github.com/KamWithK/AnkiconnectAndroid#additional-instructions-local-audio), tapi setup di PC ini tetap wajib karena audionya perlu dibuat dulu di PC

    ---

    1. Unduh semua file dari [tautan ini](https://github.com/yomidevs/local-audio-yomichan?tab=readme-ov-file#steps). Baca panduannya pelan-pelan. Kalau tidak butuh audio bahasa lain, cukup unduh audio bahasa Jepang.

    2. Buka `Tools` > `Add-ons` di Anki (++ctrl+shift+a++ di Windows, ++cmd+shift+a++ di MacOS) > `Get Add-ons...`, masukkan kode `1045800357`, lalu tutup dan buka lagi Anki

    3. Ekstrak `local-yomitan-audio-collection`, lalu tempel folder `user_files` ke:
        - Folder add-on-nya: di jendela add-on, pilih `Local Audio Server for Yomitan` > `View Files`
        - Atau ke: 
              - Windows: `C:\Users\NamaKamu\AppData\Roaming\Anki2\addons21\1045800357`
              - MacOS: `~/Library/Application Support/Anki2/addons21/1045800357` (buka lewat `Finder` > `Go` > `Go to Folder...`, lalu tempel alamat ini)

    4. Kalau kamu memakai pengaturan Yomitan dari LazyGuide:
        - Buka `Yomitan settings` > `Audio` > `Configure audio playback sources...` > `Add` > `Custom URL (JSON)`
        - Tempel `http://localhost:5050/?term={term}&reading={reading}`, lalu taruh di urutan paling atas

    5. Cek apakah sudah jalan:

        ![Yomitan Local Audio Check](img/yomitan-local-audio-check.gif){height=250 width=500}	
	Selesai!


#### Info 2: Mode Terang/Gelap Yomitan

??? info "Mode Terang & Gelap Yomitan <small>(klik di sini)</small>"

    Buka `Yomitan settings` > `Appearance` > `Theme` untuk mengganti tema.

    ![Yomitan Theme](img/yomitan-theme.png){height=300 width=600}

---

## Pertanyaan Umum

#### Pertanyaan 1: Boleh menambah atau menghapus kamus Yomitan sendiri?

??? question "Boleh menambah, menghapus, atau mengubah kamus Yomitan? <small>(klik di sini)</small>"

    - Silakan. Sebagian besar kamus berformat Yomitan bisa dipakai. Tinggal ikuti langkah 6 di bagian [Setup](setup-yomitan-pc-lazy-guide.md/#setup)

    - Kamu juga bisa mengubahnya di `Yomitan settings` > `Anki` > `Configure Anki card format...` > `MainDefinition`, lalu pilih `single-glossary-NAMA-KAMUS-YANG-KAMU-MAU` dari dropdown

    - Kalau mengganti `MainDefinition`, ubah juga di setiap `Profile`

#### Pertanyaan 2: Cari kamus lainnya di mana?

??? question "Cari kamus lainnya di mana? <small>(klik di sini)</small>"

    - Cek koleksi kamus lain di [koleksi Shoui](https://learnjapanese.link/dictionaries) dari TMW atau [koleksi Marv](https://drive.google.com/drive/folders/1xURpMJN7HTtSLuVs9ZtIbE7MDRCdoU29) dari Yomitan

#### Pertanyaan 3: Rekomendasi kamus frekuensi?

??? question "Rekomendasi kamus frekuensi? <small>(klik di sini)</small>"

    - JPDB
        - Daftar frekuensi dari [jpdb.io](https://jpdb.io), situs yang menganalisis banyak *light novel*, *visual novel*, anime, dan *J-drama*. Jadi, daftar ini menunjukkan seberapa sering sebuah kata muncul di media fiksi berbahasa Jepang.
    - CC100
        - Daftar frekuensi dari korpus teks internet Jepang. Kata-kata formal akan tampak lebih umum di daftar ini.  
        - Contoh: 審議会 (*council*) memiliki peringkat ke-9733 di CC100, tetapi ke-58730 di JPDB.

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

    - Kamus di panduan ini jarang diperbarui. Santai saja, isinya memang jarang berubah
        - Tujuan panduan ini supaya tetap stabil dalam jangka panjang
        - Tapi kalau mau memperbarui sendiri, boleh juga

#### Pertanyaan 6: Bagaimana cara memakai sentence card?

??? question "Bagaimana cara memakai sentence card? <small>(klik di sini)</small>"

    - Buka `Yomitan settings` > `Anki` > `Configure Anki card format...`

      ![Sentence Card 1](img/yomitan-anki-active-profile.jpg){height=300 width=600}

    - Di bagian `Expression`, gulir ke bawah, cari `IsSentenceCard`, lalu isi dengan `1`

      ![Sentence Card 2](img/yomitan-sentence-card.jpg){height=300 width=600}

    - Terapkan ke semua profil, termasuk `Monolingual`, `Bilingual`, `Android (Anime, LN & Manga)`, dan `Android (VN)`

      ![Sentence Card 3](img/yomitan-profiles.jpg){height=300 width=600}