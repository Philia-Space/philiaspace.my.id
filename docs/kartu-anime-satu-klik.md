# Kartu Anime Satu Klik - [Yomipv oleh BrenoAqua](https://github.com/BrenoAqua/Yomipv)
---

 Diunggah: 4 November 2026 – `Yaaacha`

---
Yomipv bikin kamu bisa cari arti kata dan bikin kartu Anki **langsung di dalam MPV**, tanpa keluar dari video. Gambar, audio kalimat, dan kalimatnya otomatis masuk ke kartu.

Bisa dipakai di Windows, Linux, dan macOS.

??? info "Info: lokalisasi dari dokumentasi resmi (klik di sini)"

    Halaman ini adalah terjemahan dari [README Yomipv](https://github.com/BrenoAqua/Yomipv) dan [panduan Senren](https://brenoaqua.github.io/Senren/yomipv/). Kalau ada yang beda, ikuti README di GitHub karena itu yang paling baru.

---

## Prasyarat

* [MPV](https://mpv.io/) versi 0.33.0 atau lebih baru
* [FFmpeg](https://ffmpeg.org/), untuk mengambil gambar dan audio dari video. Kalau tidak ada, Yomipv pakai encoder bawaan MPV
* Anki dengan add-on [AnkiConnect](https://ankiweb.net/shared/info/2055492159) ([Setup Anki PC](setup-anki-pc-lazy-guide.md))
* Yomitan ([Setup Yomitan PC](setup-yomitan-pc-lazy-guide.md)) dan [Yomitan Api](https://github.com/yomidevs/yomitan-api). Cara pasang Yomitan Api ada di README-nya
* `curl`, biasanya sudah ada bawaan di sistem
* Subtitle Jepang yang sudah sinkron dengan video, bisa dicari di [Jimaku.cc](https://jimaku.cc/)
* [Node.js](https://nodejs.org/), hanya kalau pasang lewat cara alternatif di bawah

### Cek prasyarat

Buka Anki dan browser yang ada Yomitan-nya dulu, lalu copy-paste perintah ini ke PowerShell (Windows) atau Terminal (Linux/macOS). Semua baris harus `OK`, kecuali `node` yang opsional. Pastikan juga versi MPV yang muncul minimal 0.33.

=== "Windows (PowerShell)"

    ```powershell
    foreach ($c in 'mpv','ffmpeg','curl.exe','node') { if (Get-Command $c -ErrorAction SilentlyContinue) { "OK         $c" } else { "TIDAK ADA  $c" } }
    if (Get-Command mpv -ErrorAction SilentlyContinue) { mpv --version | Select-Object -First 1 }
    if (Test-Path "$env:APPDATA\mpv") { "OK         folder MPV" } else { "TIDAK ADA  folder MPV ($env:APPDATA\mpv)" }
    try { Invoke-RestMethod http://127.0.0.1:8765 | Out-Null; "OK         AnkiConnect" } catch { "TIDAK ADA  AnkiConnect (buka Anki dulu)" }
    try { Invoke-RestMethod http://127.0.0.1:19633/serverVersion -Method Post | Out-Null; "OK         Yomitan Api" } catch { "TIDAK ADA  Yomitan Api (buka browser yang ada Yomitan-nya)" }
    ```

=== "Linux/macOS (Terminal)"

    ```bash
    for c in mpv ffmpeg curl unzip grep sed node; do command -v "$c" >/dev/null && echo "OK         $c" || echo "TIDAK ADA  $c"; done
    command -v mpv >/dev/null && mpv --version | head -n 1
    [ -d ~/.config/mpv ] && echo "OK         folder MPV" || echo "TIDAK ADA  folder MPV (~/.config/mpv)"
    curl -s http://127.0.0.1:8765 >/dev/null && echo "OK         AnkiConnect" || echo "TIDAK ADA  AnkiConnect (buka Anki dulu)"
    curl -s -X POST http://127.0.0.1:19633/serverVersion >/dev/null && echo "OK         Yomitan Api" || echo "TIDAK ADA  Yomitan Api (buka browser yang ada Yomitan-nya)"
    ```

Kalau ada yang `TIDAK ADA`:

* **mpv / ffmpeg / node**: pasang dulu dari tautan di atas. Kalau sudah dipasang tapi tetap `TIDAK ADA`, berarti programnya belum masuk PATH. Untuk MPV versi portable ini tidak masalah, cukup pastikan versinya minimal 0.33
* **folder MPV**: buka MPV sekali, atau buat foldernya sendiri
* **AnkiConnect**: pastikan Anki terbuka dan add-on AnkiConnect sudah terpasang
* **Yomitan Api**: pastikan `Enable Yomitan API` sudah aktif di pengaturan Yomitan (bagian General, nyalakan advanced options dulu), lalu buka ulang browsernya

---

## Instalasi

=== "Disarankan"

    1. Download [versi terbaru untuk OS kamu](https://github.com/BrenoAqua/Yomipv/releases/latest) (file `.zip` untuk Windows, Linux, atau macOS)
    2. Ekstrak isinya langsung ke folder MPV:
        - Windows: `%APPDATA%/mpv/`
        - Linux/macOS: `~/.config/mpv/` (buat foldernya kalau belum ada)

=== "Alternatif (butuh Node.js)"

    Clone repo-nya ke folder MPV lalu pasang dependensinya. Pastikan Node.js sudah terpasang.

    - Windows, jalankan di `%APPDATA%/mpv/`:
        ```
        git clone https://github.com/BrenoAqua/Yomipv && xcopy /e /i /y Yomipv . && rd /s /q Yomipv && cd scripts\yomipv\lookup-app && npm install
        ```
    - Linux/macOS, jalankan di `~/.config/mpv/`:
        ```
        git clone https://github.com/BrenoAqua/Yomipv && cp -rn Yomipv/* . && rm -rf Yomipv && cd scripts/yomipv/lookup-app && npm install
        ```

---

## Pengaturan

1. Buka `script-opts/yomipv.conf` di folder MPV
2. Ganti nama deck, note type, dan nama field sesuai punya kamu. Bawaannya diatur untuk note type Senren. Kalau kamu pakai [Lapis](https://github.com/donkuri/lapis), ganti bagian ini:

    ```ini
    # Deck and Note type
    deck=Mining
    note_type=Lapis

    # Note fields
    expression_field=Expression
    expression_furigana_field=ExpressionFurigana
    reading_field=ExpressionReading
    pitch_accents_field=
    pitch_position_field=PitchPosition
    pitch_categories_field=PitchCategories
    sentence_field=Sentence
    sentence_furigana_field=SentenceFurigana
    secondary_sentence_field=
    expression_audio_field=ExpressionAudio
    sentence_audio_field=SentenceAudio
    selection_text_field=SelectionText
    definition_field=MainDefinition
    glossary_field=Glossary
    image_field=Picture
    freq_sort_field=FreqSort
    freq_field=Frequency
    miscinfo_field=MiscInfo
    dictionary_pref_field=
    ```

    Ganti `Mining` dengan nama deck kamu, persis sama dengan yang di Anki. Mau atur kamus mana yang masuk ke field definisi? Lihat [Pertanyaan 4](#pertanyaan-4-gimana-cara-atur-definisi-yang-masuk-ke-kartu).

3. Sebelum mulai nonton, pastikan:
    - Anki sudah dibuka dan AnkiConnect aktif
    - Yomitan Api jalan, browser yang ada Yomitan-nya terbuka, dan kamus sudah terpasang

---

## Cara Pakai

1. Buka video dengan subtitle Jepang di MPV
2. Tekan `c` untuk memunculkan pemilih kata. Bisa juga cukup gerakkan mouse setelah diam sebentar, kalau `selector_trigger_on_mouse_move` diaktifkan
3. Pilih kata dengan mengarahkan mouse atau pakai tombol panah
    - `Shift+←` / `Shift+→`: perluas pilihan ke baris subtitle sebelumnya/berikutnya
4. Tekan `Enter`, `c`, atau klik kiri untuk bikin kartu Anki. Selesai!

---

## Fitur Lain

### Pemilih kata

* **Mode gabung** (`Shift+C`): pilih beberapa baris subtitle sekaligus sebelum dijadikan kartu. Tekan `Shift+C` untuk masuk, `c` untuk mulai memilih kata, atau `Shift+C` lagi untuk batal
* **Navigasi per mora**: kalau `selector_mora_hover` aktif, arahkan mouse ke tengah kata untuk mencari mulai dari mora itu. Tekan `s` supaya tombol panah bergerak per mora, bukan per kata
* **Muncul otomatis** (`z`): pemilih kata terbuka sendiri saat mouse digerakkan setelah diam. Atur juga `selector_trigger_on_mouse_move` dan `selector_trigger_mouse_idle_time` di `yomipv.conf`
* **Mode tetap** (`v`): bikin beberapa kartu dari satu baris subtitle tanpa menutup pemilih. Warna pilihan berubah saat mode ini aktif

### Gambar dan audio

* `q` / `w`: atur sendiri waktu mulai/selesai untuk gambar dan audio. Kalau tidak diatur, ikut awal dan akhir subtitle
* `e`: hapus waktu yang diatur manual
* `g`: ganti antara gambar diam (screenshot) dan gambar bergerak (klip animasi)

### Riwayat subtitle

* `a`: buka/tutup panel riwayat subtitle
* Klik baris di riwayat untuk lompat ke adegannya (saat pemilih kata tertutup), atau untuk menambah baris sebelumnya/berikutnya ke pilihan (saat pemilih kata terbuka)
* `Alt+←` / `Alt+→`: lompat ke subtitle sebelumnya/berikutnya
* `r`: putar ulang baris subtitle saat ini dari awal lalu pause di akhir, enak buat latihan dengar
* `x`: hapus riwayat subtitle (saat panel riwayat terbuka)

### Jendela kamus

Jendela kecil berisi arti kata dari kamus Yomitan kamu, lengkap dengan pitch accent dan frekuensi. Jendela ini muncul otomatis saat kamu mengarahkan mouse ke kata.

* `Ctrl+c`: buka jendela kamus secara manual setelah memilih kata
* Klik kanan kata di pemilih untuk mengunci jendela kamus
* Klik mora mana saja di judul kata untuk mencari potongan katanya, klik kanan judul untuk kembali ke kata sebelumnya
* Atur `lookup_show_pitch_accents` dan `lookup_show_frequencies` di `yomipv.conf` untuk menampilkan/menyembunyikan pitch accent dan frekuensi
* Detail lengkap: [Pertanyaan 1](#pertanyaan-1-gimana-cara-pakai-jendela-kamus)

### Subtitle

* **Warna sesuai status kartu** (`Shift+S`): ganti antara subtitle biasa dan subtitle berwarna sesuai status kartu Anki kamu (baru, sedang dipelajari, review, suspend). Makin lama interval kartunya, warnanya ikut berubah
    - Tekan `Shift+B` dulu untuk membaca koleksi Anki kamu, baru warnanya bisa muncul
    - Kata yang baru kamu jadikan kartu langsung berwarna merah di subtitle
    - Aktifkan `substitute_mpv_subtitles` di `yomipv.conf` supaya langsung aktif saat MPV dibuka
    - Aktifkan dulu `colorizer_enabled=yes` di `yomipv.conf`. Detail lengkap: [Pertanyaan 2](#pertanyaan-2-gimana-cara-kerja-warna-subtitle)
* **Sinkronkan subtitle** (`Ctrl+s`): samakan waktu subtitle Jepang dengan subtitle terjemahan kalau subtitle Jepangnya telat atau kecepatan. Tekan lagi untuk membatalkan. Aktifkan `auto_sync_subtitles` supaya jalan otomatis. Karena yang disamakan hanya waktu di awal, subtitle masih bisa meleset di tengah video
* **Subtitle kedua**: subtitle terjemahan dipilih otomatis sesuai bahasa di `primary_sub_lang` dan `secondary_sub_lang` (bawaannya Jepang dan Inggris). File `.ass`/`.srt` di folder yang sama dengan video juga ikut dicari
    - `Ctrl+j` / `Ctrl+Shift+J`: ganti subtitle kedua
    - Subtitle kedua hanya muncul saat mouse diarahkan ke subtitle. Isi `secondary_on_hover=no` supaya selalu tampil
* **Saring subtitle**: tulisan yang bukan dialog (papan nama, gambar, kode format) disembunyikan otomatis. Atur lewat `subtitle_filter_enabled`

### AniList

* `Ctrl+a`: hubungkan akun AniList supaya progres episode tercatat otomatis. Detail lengkap: [Pertanyaan 3](#pertanyaan-3-gimana-cara-menghubungkan-anilist)

### Update otomatis

* Tekan `Shift+U` di MPV, atau jalankan `yomipv-updater.bat` (Windows) / `yomipv-updater.sh` (Linux/macOS)
* Bisa pilih rilis resmi terbaru atau versi paling baru dari GitHub (main branch)
* Pengaturan di `yomipv.conf` tidak akan tertimpa
* Di Windows, updater butuh izin administrator

---

## Pemecahan Masalah

=== "Windows"

    * Pastikan PowerShell boleh menjalankan script
    * Pastikan `curl` ada di `C:\Windows\System32\curl.exe`

=== "Linux"

    * Pastikan `curl`, `unzip`, `grep`, dan `sed` sudah terpasang
    * Beri izin jalan ke updater: `chmod +x yomipv-updater.sh`
    * Pastikan file jendela kamus di `scripts/yomipv/` juga punya izin jalan

=== "macOS"

    * Pastikan `curl`, `unzip`, `grep`, dan `sed` sudah terpasang
    * Beri izin jalan ke updater: `chmod +x yomipv-updater.sh`
    * Kalau macOS memblokir jendela kamus (peringatan Gatekeeper), jalankan: `xattr -cr scripts/yomipv/YomipvLookup.app`
    * Folder MPV ada di `~/.config/mpv/` (buat kalau belum ada)

---

## Sinkronisasi Subtitle (Windows)

Kalau subtitle Jepang kamu meleset jauh dari video, sinkronkan dulu file subtitle-nya pakai [auto-sub-retimer-easy](https://github.com/shoui520/auto-sub-retimer-easy).

### Prasyarat

* Windows
* Video tersimpan di komputer (misalnya anime yang didownload dalam format .mkv)
* File subtitle Jepang di folder yang sama dengan video
* Untuk opsi 1, video harus punya subtitle bawaan (softsub). Kalau video kamu raw (tanpa softsub), pakai opsi 2 yang berbasis audio

### Instalasi

1. Instal Python. Download [di sini](https://www.python.org/ftp/python/3.14.2/python-3.14.2-amd64.exe)
2. Buka [auto-sub-retimer-easy](https://github.com/shoui520/auto-sub-retimer-easy), klik tombol hijau "**Code**", lalu "**Download ZIP**"
3. Ekstrak file .zip dengan klik "**Extract all**"
4. Di dalamnya ada folder `auto-sub-retimer-easy-master`. Pindahkan folder ini langsung ke `C:\`. **Ini langkah penting!**
    - Benar: `C:\auto-sub-retimer-easy-master`, dengan `Install.reg`, `ffmpeg`, dll. langsung di dalamnya
    - Salah: `C:\auto-sub-retimer-easy-master\auto-sub-retimer-easy-master`
5. Klik dua kali `Install.reg` lalu tekan "Yes". Langkah ini butuh izin administrator

### Penggunaan

1. Taruh file subtitle (misalnya dari Jimaku.cc) di folder yang sama dengan video. Jumlah subtitle harus sama dengan jumlah episode (misalnya 24 episode, 24 subtitle)
2. Klik kanan folder video+subtitle di File Explorer, lalu "Show more options" (di Windows 11)
3. Arahkan ke "Retime/Rename Subs" lalu klik "RetimeSubs"
4. Jendela terminal akan muncul dengan pilihan:
    - `[1]` Retime using embedded subs (bawaan, cocok untuk kebanyakan kasus)
    - `[2]` Retime using audio
5. Ketik nomornya lalu tekan Enter
6. Kalau ditanya "Split Penalty", langsung tekan Enter saja
7. Kalau ditanya "styles to keep", tekan Enter juga
8. Tunggu sampai muncul tulisan "Success!"

Kadang subtitle Inggris dan Jepang isinya tidak sama, misalnya subtitle Inggris menerjemahkan tulisan dan lagu, sedangkan subtitle Jepang berisi teks untuk tunarungu. Untuk kasus seperti itu, atau kalau videonya raw, pakai opsi `[2]`.

---

## FAQs

#### Pertanyaan 1: Gimana cara pakai jendela kamus?

??? question "Gimana cara pakai jendela kamus? <small>(klik untuk buka)</small>"

    Jendela kamus (Lookup App) menampilkan arti, pitch accent, dan frekuensi kata yang kamu pilih di MPV. Semua datanya diambil dari kamus yang terpasang di Yomitan.

    **Cara memunculkan**

    - **Otomatis**: muncul saat mouse diarahkan ke kata di pemilih. Matikan lewat `selector_lookup_on_hover=no`
        - Aktifkan `selector_lookup_on_navigation=yes` supaya jendela juga muncul saat pindah kata pakai tombol panah
    - **Manual**: tekan `Ctrl+c` sambil mengarahkan mouse ke kata di pemilih

    Jendela ini tetap di atas MPV sampai kartu dibuat atau pemilih dibatalkan. Klik kanan kata di pemilih untuk **mengunci** jendela, supaya isinya tidak berganti saat mouse lewat kata lain.

    **Menu klik kanan** (klik kanan di dalam jendela kamus)

    - **Copy**: salin teks yang sedang dipilih
    - **Inspect Element**: buka developer tools jendela kamus
    - **Refresh CSS**: muat ulang tampilan dari `yomipv.css`

    **Urutan hasil**

    - Bawaannya, kata yang paling panjang cocok ditampilkan dulu, sama seperti Yomitan. Jadi bentuk konjugasi dan kata majemuk muncul sebelum potongan katanya
    - Isi `prioritize_kanji_match=yes` kalau mau entri yang ada kanjinya didahulukan
    - Kalau hasilnya lebih dari satu, ada penanda seperti `1 / 3` di atas. Klik tombol kiri/kanan di jendela untuk ganti entri

    **Mencari potongan kata**

    - Klik mora mana saja di judul kata untuk mencari mulai dari situ
    - Klik kanan judul kata untuk kembali ke kata sebelumnya

    **Memilih isi definisi untuk kartu**

    - Blok teks di dalam definisi untuk mengisi field `SelectionText` di Anki, sama seperti di popup Yomitan. Ini berlaku kalau kamu pakai `popup-selection-text` (lihat [Pertanyaan 4](#pertanyaan-4-gimana-cara-atur-definisi-yang-masuk-ke-kartu))
    - `Ctrl+c` saat ada teks terpilih akan menyalin teks itu dan menghapus pilihannya
    - Klik **judul kamus** untuk memakai kamus itu sebagai isi field definisi, kalau kamu pakai `selected-dict`. Setelah kamus dipilih, `popup-selection-text` diabaikan, dan teks yang kamu blok di definisi akan di-highlight

    **Pitch accent dan frekuensi**

    - Bawaannya tampil. Kata juga diwarnai sesuai pola pitch accent-nya
    - Sembunyikan lewat `lookup_show_pitch_accents=no` atau `lookup_show_frequencies=no`

    **Ganti tampilan**

    1. Buka `script-opts/yomipv.css`
    2. Tambahkan CSS kamu sendiri
    3. Klik kanan di jendela kamus > **Refresh CSS** untuk melihat hasilnya tanpa restart MPV

    File ini tidak akan tertimpa saat update.

    **Inspect Element**

    - Klik kanan > **Inspect Element** membuka jendela DevTools di bagian Elements
    - Selama Inspector terbuka, jendela kamus bisa digeser ke mana saja. Setelah Inspector ditutup, jendela kembali ke posisi semula
    - Selama Inspector aktif ada ikon di system tray, buat memunculkan lagi jendela yang ter-minimize

    Sumber: [lookup-app.md](https://github.com/BrenoAqua/Yomipv/blob/main/docs/lookup-app.md)

#### Pertanyaan 2: Gimana cara kerja warna subtitle?

??? question "Gimana cara kerja warna subtitle? <small>(klik untuk buka)</small>"

    Fitur ini (Colorizer) mewarnai kata di subtitle sesuai status kartunya di Anki, jadi kamu langsung tahu kata mana yang baru, sedang dipelajari, atau sudah hafal.

    **Arti warna**

    - **Abu-abu**: kartu di-suspend
    - **Merah**: kata baru, belum dipelajari
    - **Oranye ke kuning**: sedang dipelajari (interval sampai 21 hari)
    - **Hijau ke biru muda**: sudah hafal (interval sampai 2000 hari)

    ![Contoh warna subtitle Yomipv](https://raw.githubusercontent.com/BrenoAqua/Yomipv/main/docs/assets/colorizer_example.png){width=600}

    **Cara mengaktifkan**

    1. Pastikan Anki terbuka dan AnkiConnect aktif
    2. Ubah pengaturan ini di `script-opts/yomipv.conf`. Bawaannya `colorizer_enabled=no`, jadi wajib diganti:

        ```ini
        # Aktifkan colorizer
        colorizer_enabled=yes

        # Warnai katanya
        selector_colorize_words=yes

        # Kasih garis bawah berwarna, bukan mewarnai teksnya
        selector_colorize_underline=no
        ```

    3. Isi `ankidb_word_fields` dengan nama field yang berisi kata Jepang di note type kamu. Supaya pencocokan kana lebih akurat, isi juga `ankidb_reading_fields` dengan field cara bacanya. Untuk Lapis:

        ```ini
        ankidb_word_fields=Expression
        ankidb_reading_fields=ExpressionReading
        ```

    4. Tekan `Shift+B` minimal sekali untuk membaca koleksi Anki kamu
    5. Tekan `Shift+S` untuk ganti antara subtitle biasa dan subtitle berwarna

    **Perlu diingat**

    - Yomipv menyimpan salinan data Anki kamu di `anki_words.json` supaya cepat. Salinan ini **tidak** ter-update sendiri, jadi tekan `Shift+B` lagi kalau mau warnanya ikut progres Anki terbaru
    - Kata yang baru kamu jadikan kartu langsung masuk ke salinan ini dan berwarna merah
    - Warna hanya muncul kalau subtitle utama berbahasa Jepang. Yomipv mengeceknya dari label bahasa subtitle (`ja`, `jp`, `jpn`, `japanese`, atau `日本語`). Kalau subtitle tidak punya label bahasa, Yomipv mengecek apakah teksnya berisi huruf Jepang
    - Kalau subtitle utamanya bukan bahasa Jepang, subtitle MPV biasa tetap tampil tanpa warna

    Sumber: [colorizer.md](https://github.com/BrenoAqua/Yomipv/blob/main/docs/colorizer.md)

#### Pertanyaan 3: Gimana cara menghubungkan AniList?

??? question "Gimana cara menghubungkan AniList? <small>(klik untuk buka)</small>"

    Yomipv bisa mencatat progres episode ke akun AniList kamu secara otomatis.

    **Cara setup**

    1. Buka video apa saja di MPV
    2. Tekan `Ctrl+a` (atau tombol yang kamu atur di `key_anilist_auth`)
    3. Browser akan membuka halaman izin AniList, dan jendela terminal muncul bersamaan
    4. Klik **Approve** di browser
    5. Copy seluruh URL dari address bar
    6. Paste ke terminal lalu tekan Enter
    7. Token akan disimpan ke `yomipv.conf` dan pencatatan diaktifkan
    8. Restart MPV supaya mulai jalan

    **Fitur**

    - **Otomatis**: progres di-update setelah video ditonton melewati `anilist_update_thresh_percent` (bawaannya 80%)
    - **Nomor episode diubah otomatis**: nomor episode berurutan seperti *Re Zero kara Hajimeru Isekai Seikatsu - 67* diubah ke format per season AniList (*Season 4 Episode 1*). Tidak perlu diatur manual
    - **Notifikasi**: atur notifikasi di layar lewat `anilist_show_notifications`. Lompat-lompat di timeline tidak akan mengirim update berkali-kali

    Sumber: [anilist_tracking.md](https://github.com/BrenoAqua/Yomipv/blob/main/docs/anilist_tracking.md)

#### Pertanyaan 4: Gimana cara atur definisi yang masuk ke kartu?

??? question "Gimana cara atur definisi yang masuk ke kartu? <small>(klik untuk buka)</small>"

    Isi field definisi, `SelectionText`, dan glossary di kartu diatur lewat tiga pengaturan ini di `yomipv.conf`:

    ```ini
    selection_text_handlebar=popup-selection-text
    definition_handlebar=selected-dict
    glossary_handlebar=glossary
    ```

    Kosongkan nilainya kalau tidak mau field itu diisi.

    **Penanda dari Yomitan**

    Penanda (marker) yang bisa dipakai sama dengan di Yomitan:

    `glossary`, `glossary-brief`, `glossary-no-dictionary`, `glossary-plain`, `glossary-plain-no-dictionary`, `glossary-first`, `glossary-first-brief`, `glossary-first-no-dictionary`, `single-glossary-NAMA-KAMUS`, `single-glossary-NAMA-KAMUS-brief`, `single-glossary-NAMA-KAMUS-no-dictionary`, `popup-selection-text`

    Contoh:

    ```ini
    definition_handlebar=popup-selection-text
    definition_handlebar=single-glossary-NAMA-KAMUS
    definition_handlebar=glossary
    ```

    Hasilnya sama seperti saat membuat kartu dari popup Yomitan. Kalau ada kamus yang dipilih lewat `selected-dict`, `popup-selection-text` tidak dipakai.

    **Penanda khusus Yomipv: `selected-dict`**

    Di jendela kamus, klik judul kamus untuk menjadikannya **kamus pilihan**. Penanda `selected-dict` mengisi field dengan isi kamus itu.

    - Kalau ada kamus yang dipilih, isinya masuk ke field tersebut
    - Kalau tidak ada, Yomipv pakai penanda cadangan berikutnya
    - Teks yang kamu blok di dalam entri kamus akan di-highlight

    **Pakai cadangan**

    Bisa isi beberapa penanda dipisah koma. Yomipv mencoba dari kiri ke kanan:

    ```ini
    definition_handlebar=selected-dict,single-glossary-NAMA-KAMUS
    ```

    Kalau ada kamus yang dipilih di jendela kamus, itu yang dipakai. Kalau tidak, pakai `single-glossary-NAMA-KAMUS`.

    **Handlebar sendiri**

    Handlebar buatan sendiri juga bisa, termasuk dari [handlebar kamus AuroraWright](https://gist.github.com/AuroraWright/8f529e7ec5a47bfa5d979821541562a5):

    ```ini
    definition_handlebar=selected-dict,primary-definition
    definition_handlebar=selected-dict,secondary-definition
    ```

    Aturan ini (beberapa penanda dipisah koma, dicoba dari kiri ke kanan, `selected-dict`, dan handlebar sendiri) berlaku untuk ketiga pengaturan: `definition_handlebar`, `selection_text_handlebar`, dan `glossary_handlebar`.

    Sumber: [field_handlebars.md](https://github.com/BrenoAqua/Yomipv/blob/main/docs/field_handlebars.md)
