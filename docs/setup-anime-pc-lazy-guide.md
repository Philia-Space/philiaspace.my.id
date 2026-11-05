
# Setup Mining Anime di PC
---

 Diunggah: 18 Januari 2026 · Diperbarui: 5 November 2026 – `Yaaacha`

---
## Permulaan

- asbplayer adalah pemutar video di browser untuk menonton anime beserta subtitle-nya. Kata di subtitle bisa dicari dengan Yomitan cukup dengan mengarahkan kursor.
- animetan adalah fork dari asbplayer dengan tambahan fitur memasukkan subtitle secara otomatis.

---

## Unduh & Pasang

- Akun [Jimaku](https://jimaku.cc/) (bisa dilewati kalau tidak memakai animetan)
- Unduh anime dan subtitle Jepang yang mau kamu tonton
    - Subtitle Jepang bisa dicari di [Jimaku](https://jimaku.cc/)

- Untuk video streaming, pasang ekstensi [animetan](https://chromewebstore.google.com/detail/animetan-asbplayer-with-a/mmoglblloplhkmjpeckknpadfhpgjhoi)
!!! warning "Untuk Pengguna Firefox"
    Pengguna Firefox bisa memasang animetan [dari sini](https://addons.mozilla.org/en-US/firefox/addon/animetan-auto-subtitles/), tapi banyak fiturnya tidak tersedia. Lihat [catatan ini](https://docs.asbplayer.dev/docs/compatibility).


Syarat:

- [Yomitan di PC](setup-yomitan-pc-lazy-guide.md) sudah terpasang

---

## Langkah-langkah Penggunaan Video Lokal

1. Di browser, buka `chrome://flags` atau `edge://flags`
    - Cari `Experimental Web Platform features`, lalu aktifkan

    ![Aktifkan Fitur Eksperimen](img/enable-experimental-web-platform.png){height=300 width=600}

2. Buka [asbplayer](https://app.asbplayer.dev/)

3. Buka pengaturan lewat ikon gir di kanan atas, lalu samakan isinya dengan [pengaturan](setup-anime-pc-lazy-guide.md/#__tabbed_1_1) di bawah

    === "Anki"
        ![Anki Settings 1](img/asbplayer-settings-1.png){height=400 width=800}
    === "Mining"
        ![Anki Settings 2](img/asbplayer-settings-2.png){height=400 width=800}

4. Klik tombol `browse` di asbplayer, lalu pilih file anime dan subtitle-nya
    - Langkah ini tidak perlu untuk situs streaming seperti YouTube atau Netflix

    === "Buka Anime"
        ![Pick Anime PC](img/pick-anime-pc.jpg){height=300 width=600}
    === "Pilih Anime dan Sub (Win)"
        ![Pick Anime & Subtitle PC](img/pick-anime-sub.png){height=300 width=600}
    === "Pilih Anime dan Sub (Mac)"
        ![Pick Anime & Subtitle PC](img/pick-anime-sub-mac.jpg){height=300 width=600}

5. Cara mining:
    - Arahkan kursor ke kata di subtitle, lalu mining dengan Yomitan
    - Tekan ++ctrl+shift+u++ untuk menambahkan screenshot dan audio ke kartu Anki secara otomatis
    - (Opsional) Shortcut ini bisa diganti di `Settings` > `Keyboard Shortcuts` > `Update last-created Anki card`

6. Sekarang kamu sudah bisa mining dengan asbplayer dan Yomitan
    - Lihat [Demo Mining Anime](setup-anime-pc-lazy-guide.md/#info-1-demo-mining-anime)

Kamu sudah bisa mining anime di PC. Mau lanjut ke panduan Setup Mining Light Novel?

[Lanjut ke Setup Mining Light Novel di PC](setup-LN-pc-lazy-guide.md){ .md-button .md-button }

<small>Kalau ada masalah, cek [Pertanyaan Umum](setup-anime-pc-lazy-guide.md/#pertanyaan-umum)</small>

---
## Langkah-langkah Penggunaan Video Streaming

1. Buka situs nonton anime favoritmu, misalnya Hianime
2. Saat pertama kali dipakai, animetan akan menampilkan kotak untuk memasukkan API key
3. Buat akun di [jimaku.cc](https://jimaku.cc/account) untuk mendapatkan API key
4. Klik tombol `API` untuk membuat API key, lalu salin kode yang muncul
5. Tempel kode itu ke Animetan
6. Kalau judul anime di situs itu sama dengan judul di Jimaku, berikutnya animetan akan memasukkan subtitle secara otomatis


---

## Info Tambahan & Tips

#### Info 1: Demo Mining Anime

??? info "Demo Mining Anime <small>(klik di sini)</small>"

    Video demo ini memakai note type Mining-JP. Di pengaturan Anki di Yomitan, kamu seharusnya sudah memakai note type Lapis. Di video, shortcut ++ctrl+shift+x++ dipakai supaya audio, screenshot, dan subtitle bisa disunting dulu sebelum dikirim ke Anki. Kalau mau langsung memperbarui kartu terakhir yang ditambahkan Yomitan, pakai ++ctrl+shift+u++.
    <iframe width="560" height="315" src="https://youtube.com/embed/1mOGv9hAHDc" title="Mining Demo" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

#### Tip 1: Sinkronisasi Subtitle

??? tip "Sinkronisasi Subtitle <small>(klik di sini)</small>"

    Kadang subtitle tidak pas dengan videonya karena sumber anime-nya berbeda. Untuk menggesernya:

    - +100ms = ++ctrl+shift+left++
    - -100ms = ++ctrl+shift+right++

#### Tip 2: Lewatkan Rekaman Audio saat Mining

??? tip "Lewatkan Rekaman Audio saat Mining <small>(klik di sini)</small>"

    - Rekaman audio bisa dilewati supaya mining lebih cepat
    - Kalau kartu Anki dibuat kurang dari 5 detik, rekaman audionya bisa hampir tidak terdengar

#### Tip 3: ASBPlayer di Youtube, Netflix, dan Web lain

??? tip "asbplayer bisa dipakai di YouTube, Netflix, dan situs lain <small>(klik di sini)</small>"

    - Buka video yang mau diputar, tekan tombol `` ` `` (tanda petik terbalik, di samping angka 1), lalu klik `Load Subtitles`
    - Kamu bisa menampilkan hingga 3 subtitle sekaligus, dari subtitle bawaan situsnya atau dari file `.srt` yang kamu impor
    - Daftar situs lain yang didukung ada di [dokumentasi asbplayer](https://docs.asbplayer.dev/docs/compatibility#streaming-services-and-subtitle-detection)

---

## Pertanyaan Umum

#### Pertanyaan 1: Kenapa harus aktifkan Experimental Web Platform?

??? question "Kenapa fitur eksperimen perlu diaktifkan? <small>(klik di sini)</small>"

    - Beberapa file anime punya lebih dari satu audio, misalnya Jepang dan Inggris. Dengan fitur ini, kamu bisa memilih audio Jepang kalau audio bawaannya bukan Jepang

#### Pertanyaan 2: Muncul error, cek di mana?

??? question "Muncul error tertentu saat mining di asbplayer <small>(klik di sini)</small>"

    - Cek dulu [_Common Issues_ di dokumentasi asbplayer](https://docs.asbplayer.dev/docs/common-issues). Kalau masalahmu tidak ada di sana, tanyakan di [server Discord Philia Space](https://discord.com/channels/1370274344571240552/1376885138352242688)
