# Setup Mining Light Novel dan sejenisnya [LazyGuide](https://lazyguidejp.github.io/jp-lazy-guide/setupLnOnPC/)
---

 Diunggah: 10 Agustus 2025 · Diperbarui: 6 November 2026 – `Yaaacha`

---

- Kamu bisa membaca light novel di PC selama punya file EPUB-nya, situs untuk membuka EPUB, dan Yomitan yang sudah terpasang.

---

## Persyaratan

- Unduh light novel pilihanmu dalam format EPUB

- [Yomitan di PC](setup-yomitan-pc-lazy-guide.md) sudah terpasang dan diatur

---

## Cara Setup

1. Di browser, buka [Yatsu Reader](https://app.yatsu.moe/)

    ![Yatsu Reader](img/ttu-reader.png){height=500 width=1000}

2. Klik `Import` (kanan atas), lalu pilih `Import File(s)` atau `Import Folder(s)` dan pilih file atau folder EPUB light novel-mu
    - Bisa juga dengan menyeret file EPUB langsung ke halaman `Library`

    ![Yatsu Reader Import](img/ttu-upload.png){height=250 width=315}

3. Sekarang kamu bisa mining dengan Yomitan seperti biasa

    ![Yatsu Reader PC](img/ttu-reader-pc.png){height=500 width=1000}

Sekarang kamu sudah bisa membaca light novel, novel, atau buku lain di PC.

<small>Kalau ada masalah, cek [FAQs](setup-LN-pc-lazy-guide.md/#pertanyaan-umum)</small>

---

## Info Tambahan dan Tips

#### Info 1: Pengaturan Yatsu Reader dari LazyGuide

??? info "Contoh pengaturan Yatsu Reader <small>(klik di sini)</small>"
    Ini contoh pengaturan Yatsu Reader di PC. Tidak wajib diikuti, sesuaikan saja dengan selera kamu. Pengaturannya dibuka lewat menu `Settings` di bagian atas.

    === "Theme"
        ![Yatsu Settings Theme](img/yatsu-settings-theme.png){height=500 width=1000}
    === "Display"
        ![Yatsu Settings Display](img/yatsu-settings-display.png){height=500 width=1000}
    === "Text Style"
        ![Yatsu Settings Text Style](img/yatsu-settings-text-style.png){height=500 width=1000}
    === "Writing"
        ![Yatsu Settings Writing](img/yatsu-settings-writing.png){height=500 width=1000}
    === "Rendering"
        ![Yatsu Settings Rendering](img/yatsu-settings-rendering.png){height=500 width=1000}
    === "Page Layout"
        ![Yatsu Settings Page Layout](img/yatsu-settings-page-layout.png){height=500 width=1000}
    === "Progress"
        ![Yatsu Settings Progress](img/yatsu-settings-progress.png){height=500 width=1000}
    === "Navigation"
        ![Yatsu Settings Navigation](img/yatsu-settings-navigation.png){height=500 width=1000}
    === "Session"
        ![Yatsu Settings Session](img/yatsu-settings-session.png){height=500 width=1000}
    === "Highlights"
        ![Yatsu Settings Highlights](img/yatsu-settings-highlights.png){height=500 width=1000}
    === "Local Storage"
        ![Yatsu Settings Local Storage](img/yatsu-settings-local-storage.png){height=500 width=1000}
    === "Import"
        ![Yatsu Settings Import](img/yatsu-settings-import.png){height=500 width=1000}
    === "Sync"
        ![Yatsu Settings Sync](img/yatsu-settings-sync.png){height=500 width=1000}
    === "Sources"
        ![Yatsu Settings Sources](img/yatsu-settings-sources.png){height=500 width=1000}
    === "Statistics"
        ![Yatsu Settings Statistics](img/yatsu-settings-statistics.png){height=500 width=1000}
    === "Sync & Merge"
        ![Yatsu Settings Sync & Merge](img/yatsu-settings-sync-merge.png){height=500 width=1000}

#### Info 2: Pola Penggantian Teks (Text Replacement Pattern)

??? info "Pola Penggantian Teks <small>(klik di sini)</small>"

    Kalau tidak memakai pengaturan dari panduan ini, masukkan pola berikut secara manual supaya teks bisa dipindai dengan akurat.

    1. Di halaman pengaturan Yomitan, nyalakan `Advanced` di pojok kiri bawah (atau gulir ke paling bawah)

    2. Di bagian `Translation`, pilih `Configure custom text replacement patterns...`

    3. Salin pola dari [tautan ini](https://pastebin.com/er57E9Hw), lalu tempel di sana

#### Info 3: Audiobook dengan Yatsu Whispersync

??? info "Baca sambil mendengarkan audiobook <small>(klik di sini)</small>"

    [Yatsu Whispersync](https://docs.yatsu.moe/ttu-whispersync/) menambahkan pemutar audiobook ke Yatsu Reader. Kalimat yang sedang dibacakan ditandai di buku, dan halaman bisa ikut bergeser sendiri.

    **Yang dibutuhkan**

    - Browser Chrome, Edge, atau Brave di PC. Browser lain bisa, tapi file audio harus dipilih ulang setiap kali halaman dimuat ulang
    - File audiobook (`.m4a`, `.m4b`, atau `.mp3`) dan subtitle-nya (`.srt` atau `.vtt`) untuk buku yang sama

    **Pasang**

    1. Pasang ekstensi [Violentmonkey](https://violentmonkey.github.io/get-it/)
    2. Buka [script Yatsu Whispersync](https://github.com/ytrms/yatsu-whispersync/releases/latest/download/yatsu-whispersync.user.js), lalu klik `Install` di halaman Violentmonkey yang muncul
    3. Muat ulang tab Yatsu Reader, lalu buka bukunya. Ikon Whispersync muncul di bagian bawah pembaca

    **Pakai untuk satu buku**

    1. Klik ikon Whispersync di bagian bawah pembaca
    2. Pilih file subtitle, lalu file audiobook-nya
    3. Buka tab `Match`, lalu cocokkan subtitle dengan teks buku
    4. Klik `Save & reload page` saat diminta
    5. Setelah halaman dimuat ulang, buka lagi menu Whispersync untuk mulai memutar audio

    File audio tetap di komputermu dan tidak diunggah ke Yatsu.

    **Kirim kalimat dan audio ke Anki (opsional)**

    Whispersync bisa membuat kartu lewat AnkiConnect. Tambahkan alamat Yatsu ke pengaturan AnkiConnect di Anki: `Tools` > `Add-ons` > pilih `AnkiConnect` > `Config`, lalu tambahkan `"https://app.yatsu.moe"` ke daftar `webCorsOriginList`. Setelah itu, atur dek dan note type di menu Whispersync.

    Kalau ikon Whispersync tidak muncul atau audionya tidak pas, cek [bagian Troubleshooting di dokumentasi Yatsu](https://docs.yatsu.moe/ttu-whispersync/#troubleshooting).

---

## Pertanyaan Umum
