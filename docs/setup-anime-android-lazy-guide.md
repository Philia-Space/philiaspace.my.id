# Setup Mining Anime di Android [Lazy Guide](https://lazyguidejp.github.io/jp-lazy-guide/setupAnimeOnAndroid/)
---

 Diunggah: 24 Agustus 2025 · Diperbarui: 5 November 2026 – `Yaaacha`

---

- `asbplayer` adalah pemutar video di browser yang bisa memutar anime beserta subtitle-nya, supaya kamu bisa hover kata di subtitle dan memakai Yomitan.

---

## Unduh dan Pasang

- Unduh anime dan subtitle Jepang kamu  
    - Subtitle Jepang bisa diambil di [Jimaku](https://jimaku.cc/)

- (Opsional) Untuk video streaming, pasang ekstensi [asbplayer](https://chromewebstore.google.com/detail/asbplayer-language-learni/hkledmpjpaehamkiehglnbelcpdflcab)

  **Syarat:**

  - [Yomitan di Android](setup-yomitan-android-lazy-guide.md) sudah terpasang

---

## Pengaturan Awal

1. Di browser, buka `edge://flags`  
    - Cari `Experimental Web Platform features`, lalu ubah jadi `Enabled`

    ![Enable Experimental Web Platform Android](img/enable-experimental-web-platform-android.png){height=200 width=400}

2. Buka [asbplayer](https://app.asbplayer.dev/)  
    - Abaikan permintaan izin (`request permission`) ke Anki dan tawaran memasang ekstensi Chrome

3. Unggah file anime dan subtitle kamu ke `asbplayer` dengan menekan `browse`  
    - Langkah ini tidak berlaku untuk platform streaming seperti `Youtube` atau `Netflix`

    === "Upload Files"
        ![Pick Anime Android](img/pick-anime-pc.jpg){height=200 width=400}
    === "Pick Anime and Sub"
        ![Pick Anime & Subtitle Android](img/pick-anime-sub-android.png){height=200 width=400}

4. Putar HP ke posisi landscape supaya tampilan `asbplayer` pas, lalu tekan tombol di kanan atas untuk masuk mode layar penuh

    ![Android Player Buttons](img/android-player-buttons.png){height=400 width=800}

5. Sekarang kamu bisa mining pakai Yomitan dengan hover di kata-kata subtitle  
    - Lihat [Demo Mining Anime](setup-anime-pc-lazy-guide.md/#info-1-demo-mining-anime) (untuk PC)  
    - Sayangnya, untuk mengisi `Picture`, kamu harus screenshot manual lalu mengunggahnya ke detail kartu di Ankidroid

    ![Android Player Mining](img/android-player-mining.png){height=400 width=800}

Setup mining anime di Android selesai.

<small>Kalau ada masalah, cek [FAQs](setup-anime-android-lazy-guide.md/#pertanyaan-umum)</small>

---

## Info Tambahan dan Tips

#### Info 1: Demo Mining Anime (Untuk PC)

??? info "Demo Mining Anime <small>(klik di sini)</small>"

    Video ini memakai note type Mining-JP. Di pengaturan Anki di Yomitan, kamu seharusnya sudah memakai note type Lapis. Di video, pintasan ++ctrl+shift+x++ dipakai untuk mengedit audio, screenshot, dan subtitle yang akan dikirim ke Anki.
    <iframe width="560" height="315" src="https://youtube.com/embed/1mOGv9hAHDc" title="Mining Demo" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


#### Tip 1: Sinkronisasi Subtitle

??? tip "Sinkronisasi Subtitle <small>(klik di sini)</small>"

    Tergantung sumber anime kamu, subtitle bisa saja tidak sinkron. Untuk menyesuaikannya:

    - +100ms = ++ctrl+shift+left++
    - -100ms = ++ctrl+shift+right++

#### Tip 2: Lewati Rekaman Audio saat Mining

??? tip "Lewati rekaman audio saat mining <small>(klik di sini)</small>"

    - Rekaman audio bisa dilewati saat mining supaya tidak makan waktu
    - Kalau kamu bisa menjawab satu kartu Anki dalam waktu kurang dari 5 detik, audionya hampir tidak akan terpakai

---

## Pertanyaan Umum

#### Pertanyaan 1: Bagaimana cara memakai Monolingual Setup di Android?

??? question "Bagaimana cara memakai Monolingual Setup di Android? <small>(klik di sini)</small>"

    1. Buka `Yomitan settings` > `Dictionary`, lalu nyalakan `all`

        ![Dictionary Toggle](img/dictionary-toggle.png){height=250 width=500}

#### Pertanyaan 2: Kenapa Harus Menyalakan Experimental Web Platform features?

??? question "Kenapa harus menyalakan Experimental Web Platform features? <small>(klik di sini)</small>"

    - Beberapa anime punya lebih dari satu sumber audio, misalnya `en` dan `jp`. Dengan fitur ini, kamu bisa memilih `jp` kalau itu bukan audio bawaannya.

#### Pertanyaan 3: Kenapa Abaikan Request Permission ke Anki?

??? question "Kenapa request permission ke Anki diabaikan? <small>(klik di sini)</small>"

    - Karena panduan ini memakai cara biasa, supaya semua fitur Anki dan Yomitan tetap bisa dipakai.

#### Pertanyaan 4: Kenapa Tidak Memasang Chrome Extension?

??? question "Kenapa tidak memasang ekstensi Chrome? <small>(klik di sini)</small>"

    - Alasannya sama dengan Pertanyaan 3. Ekstensi `asbplayer` punya dukungan Anki bawaan, tapi fiturnya tidak selengkap setup Anki + Yomitan di panduan ini.
