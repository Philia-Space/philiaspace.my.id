<!-- upstream: setupShareX @ 2025-11-27 -->
# Setup ShareX di Windows [Lazy Guide](https://lazyguidejp.github.io/jp-lazy-guide/setupShareX/)

---

 Diunggah: 24 Agustus 2025 · Diperbarui: 5 November 2026 – `Yaaacha`

---

- ShareX adalah alat untuk mengambil screenshot, merekam audio, dan menjalankan OCR secara otomatis, supaya hasilnya bisa langsung ditempel ke kartu Anki.
- **Wajib** untuk semua metode mining di Lazy Guide.

---

## Unduh dan Pasang

- Pasang [ShareX](https://getsharex.com/)
- Unduh [lazyGuide-ShareX-settings-17.0.0](https://drive.google.com/drive/folders/1vxkbfe7tr27NxWP5baFaLLmqnExt-3Ba?usp=sharing)  
    - Bisa dipakai juga di versi ShareX yang lebih baru

---

## Cara Setup

1. Buka `ShareX` > `Application Settings` > `Settings` > `Import`, lalu pilih `lazyGuide-ShareX-settings`
    - Abaikan file dengan nama acak (isinya kosong). File itu sisa ekspor yang tidak bisa dihapus

2. Buka `ShareX` > `Hotkey Settings`, lalu ganti tombol pintas atau namanya kalau mau

     ![ShareX Hotkeys](img/sharex-hotkeys.png){height=300 width=600}

3. Cari hotkey berikut di `Hotkey Settings`:
     - `screenshot`
     - `screenshot snip`
     - `screenshot nsfw`
     - `screenshot nsfw snip`
     - `audio`
        - Untuk tiap hotkey di atas, klik ikon gir > `override screenshot folder`, lalu ubah `path`-nya
        - Ganti `LazyGuide` jadi nama profil Anki kamu:  
         `%ApplicationData%\Anki2\NamaProfilAnkiKamu\collection.media`
            - Nama profil bisa dilihat di pojok kiri atas Anki, atau lewat `File` > `Profile`
 
             ![ShareX Path](img/sharex-path.png){height=150 width=300}

4. Untuk `audio`, buka `Hotkey settings` > `audio` > `screen recorder` > `screen recorder options`  
     - Klik `Install recorder devices`
     - Ubah `Video source` jadi `none`
     - Ubah `Audio source` jadi `virtual-audio-capturer`

5. Mining kata lewat Yomitan dulu, baru pakai hotkey `screenshot` atau `audio record` di ShareX
     - Pastikan Anki sedang terbuka supaya tombol `Add(+)` muncul
     - Lihat juga [Mining Demo](setup-ShareX-pc.md/#info-1-mining-demo)

Setup ShareX selesai!

<small>Kalau ada masalah, cek [FAQs](setup-ShareX-pc.md/#pertanyaan-umum)</small>

---

## Extra Info dan Tips

#### Info 1: Mining Demo

??? info "Mining Demo <small>(klik di sini)</small>"

    Jangan lupa tonton Mining Demo!
    
    <iframe width="560" height="315" src="https://www.youtube.com/embed/tUiXU2gn75g" title="Mining Demo" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

#### Info 2: Fungsi Hotkey

??? info "Fungsi Hotkey <small>(klik di sini)</small>"

    - `screenshot` dan `screenshot nsfw`: mengambil screenshot seluruh layar utama  
        - Untuk ganti monitor, buka `Hotkey settings` > `screenshot` > `Capture` > `Select region...`

    - `screenshot snip` dan `screenshot nsfw snip`: mengambil screenshot sebagian layar (mirip crop)

    - `OCR (manga_ocr)` dipakai di [Setup OCR (owocr)](setup-manga-pc-lazy-guide.md/#setup-ocr), sedangkan `OCR` adalah OCR bawaan ShareX

#### Tip 1: Skip Rekam Audio saat Mining

??? tip "Skip Rekam Audio saat Mining <small>(klik di sini)</small>"

    - Rekam audio boleh dilewati kalau terasa makan waktu
    - Kalau kamu bisa membuat satu kartu Anki dalam waktu kurang dari 5 detik, audio rekamannya hampir tidak akan terdengar

---

## Mining Satu Tangan pakai Mouse

??? info "Mining Satu Tangan pakai Mouse <small>(klik di sini)</small>"

    Pasang [Autohotkey](https://www.autohotkey.com/)

    Unduh dan jalankan hotkey-nya dari [sini](https://drive.google.com/drive/folders/1ex79TQF7yAliekkR_4q3LK6PhueSM_wK?usp=sharing)

    #### Opsi 1: ALT + Screenshot Hotkey
    - Tombol Forward Mouse = ++alt++ (untuk pop-up monolingual)
    - Tombol Back Mouse = Screenshot (non-NSFW)

    #### Opsi 2: Audio + Screenshot Hotkey
    - Tombol Forward Mouse = Rekam audio
    - Tombol Back Mouse = Screenshot (non-NSFW)

    #### Opsi 3: Screenshot (NSFW) + Screenshot (non-NSFW) Hotkey
    - Tombol Forward Mouse = Screenshot
    - Tombol Back Mouse = Screenshot (non-NSFW)

---

## Pertanyaan Umum
