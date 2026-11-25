---
description: "Daftar note type Anki untuk mining bahasa Jepang (Lapis, Kiku, Senren, jp-mining-note, dan lainnya), lengkap dengan gambar contoh kartunya."
---
# Pilihan Note Type

Note type adalah desain dan susunan kolom (field) kartu Anki. Note type menentukan apa yang muncul di depan dan belakang kartu, dan field apa saja yang diisi Yomitan saat kamu mining.

Halaman ini mengumpulkan note type untuk mining bahasa Jepang, lengkap dengan gambar contohnya. Kalau bingung, pakai **Lapis**: note type ini yang dipakai hampir semua panduan di situs ini.

??? info "Tentang daftar ini <small>(klik di sini)</small>"
    - Susunan halaman ini mengikuti [Alternatives](https://aquafina-water-bottle.github.io/jp-mining-note/alternatives/) di dokumentasi jp-mining-note, ditambah note type yang lebih baru, termasuk yang dibagikan di channel #resources-sharing server Discord [TheMoeWay](https://learnjapanese.moe/join/).
    - Semua gambar dan video contoh diambil langsung dari situs atau repositori pembuat note type-nya, jadi tampilannya bisa sedikit berbeda dengan versi terbaru.
    - Note type di bagian [Note Type Lama](#note-type-lama) sebagian besar sudah tidak dirawat. Tetap boleh dipakai, tapi cek dulu apakah masih jalan di Anki dan Yomitan versi terbaru.
    - Cara mengisi field untuk Lapis, Kiku, Senren, dan Mining-JP ada di [Pengaturan Note Type](pengaturan-note-type.md). Cara memperbaruinya ada di [Memperbarui Note Type](pembaruan-note-type.md).
    - Mau pindah note type tanpa kehilangan jadwal ulasan? Lihat [Pindah ke jp-mining-note](pindah-ke-jp-mining-note.md). Langkah ganti note type di sana juga berlaku untuk note type lain.

---

## Dipakai di Philia Space

### Lapis

| | |
|---|---|
| Situs | [GitHub](https://github.com/donkuri/lapis) |
| Unduh | [Rilis terbaru](https://github.com/donkuri/lapis/releases/latest) (`Lapis.apkg`) |
| Dipakai di | Hampir semua panduan, mulai dari [Setup Anki PC](setup-anki-pc-lazy-guide.md) |

Note type yang ringan, cepat, dan cocok dengan banyak alat. Tidak butuh template Yomitan khusus, jadi bisa dipakai dengan kamus apa pun. Jenis kartu (kosakata, kalimat, klik, audio) dipilih lewat field `Is...Card`. **Paling direkomendasikan.**

![Contoh kartu Lapis: klik pinggir definisi untuk ganti kamus, arahkan kursor ke kalimat untuk furigana](https://raw.githubusercontent.com/donkuri/lapis/main/assets/Lapis.gif){ loading=lazy }

### Kiku

| | |
|---|---|
| Situs | [Dokumentasi](https://kiku.youyoumu.my.id/) · [GitHub](https://github.com/youyoumu/kiku) |
| Unduh | [Rilis terbaru](https://github.com/youyoumu/kiku/releases/latest), butuh add-on [Kiku Note Manager](https://ankiweb.net/shared/info/408592650) |
| Dipakai di | Opsional di [Manatan](Setup-Manatan.md) |

Note type yang sangat interaktif. Fitur utamanya *Kanji Web* (melihat kartu lain yang memakai kanji atau bacaan yang sama), penggabungan beberapa kalimat dan gambar ke satu kartu, puluhan tema, dan halaman pengaturan. Field-nya sama dengan Lapis, tapi butuh Anki desktop untuk memasang dan memperbaruinya. Ada [demo langsung](https://kiku.youyoumu.my.id/) di dokumentasinya.

=== "Kanji Web"

    <video controls muted preload="metadata" width="100%" src="https://kiku.youyoumu.my.id/media/feature-kanji-web.webm"></video>

=== "Tema"

    <video controls muted preload="metadata" width="100%" src="https://kiku.youyoumu.my.id/media/feature-theme.2.webm"></video>

### Senren

| | |
|---|---|
| Situs | [Dokumentasi](https://brenoaqua.github.io/Senren/) · [GitHub](https://github.com/BrenoAqua/Senren) |
| Unduh | [Rilis terbaru](https://github.com/BrenoAqua/Senren/releases/latest) |
| Dipakai di | Bawaan Yomipv di [Kartu Anime Satu Klik](kartu-anime-satu-klik.md) |

Note type yang mudah diatur dengan tampilan responsif dan animasi halus. Satu kartu bisa menyimpan beberapa adegan (kalimat, gambar, dan audio) untuk kata yang sama, lalu kamu bisa berpindah adegan saat mengulas. Ada juga pewarnaan kamus, mode gelap sendiri, dan blur gambar NSFW.

=== "PC"

    ![Tampilan bawaan Senren di PC](https://brenoaqua.github.io/Senren/assets/images/Layout_Default.png){ loading=lazy }

=== "HP"

    ![Tampilan Senren di HP](https://brenoaqua.github.io/Senren/assets/images/Mobile_Layout_1.jpg){ loading=lazy width=360 }

=== "Demo"

    <video controls muted preload="metadata" width="100%" src="https://brenoaqua.github.io/Senren/assets/demo.mp4"></video>

### Mining-JP (JP-study)

| | |
|---|---|
| Situs | [GitHub](https://github.com/rudnam/JP-study#anki-mining-template) |
| Unduh | [Mining_temp.apkg](https://github.com/rudnam/JP-study/raw/main/Mining_temp.apkg) |
| Dipakai di | [Setup Yomitan & Anki PC](setup-yomitan-pc.md) dan contoh di panduan anime |

Template mining sederhana buatan rudnam. Kartu kosakata dan kartu kalimat dipilih lewat field `*IsSentenceCard`. Warna kartunya bisa mengikuti tema sistem, dan sudah ada pemetaan field untuk mpvacious dan jidoujisho.

=== "Demo"

    ![Demo note type Mining-JP](https://raw.githubusercontent.com/rudnam/JP-study/main/images/mining_template.gif){ loading=lazy }

=== "Kartu kosakata"

    ![Belakang kartu kosakata Mining-JP](https://raw.githubusercontent.com/rudnam/JP-study/main/images/vocab_back.png){ loading=lazy }

=== "Kartu kalimat"

    ![Belakang kartu kalimat Mining-JP](https://raw.githubusercontent.com/rudnam/JP-study/main/images/sentence_back.png){ loading=lazy }

---

## Note Type Lain

### jp-mining-note

| | |
|---|---|
| Situs | [Dokumentasi](https://aquafina-water-bottle.github.io/jp-mining-note/) · [GitHub](https://github.com/Aquafina-water-bottle/jp-mining-note) |
| Unduh | [Setup](https://aquafina-water-bottle.github.io/jp-mining-note/setup/) · [fork arbyste](https://arbyste.github.io/jp-mining-note-prerelease/) (perbaikan untuk AJT Japanese terbaru) |
| Pindah ke sini | [Pindah ke jp-mining-note](pindah-ke-jp-mining-note.md) |

Note type yang sangat kaya fitur: pitch accent berwarna, tooltip kata lain yang memakai kanji yang sama, banyak jenis kartu, dan bisa diubah tampilannya sampai ke kode. Pengaturannya lebih rumit daripada Lapis, dan tidak dirancang untuk HP. Dokumentasi aslinya terakhir diperbarui tahun 2023, dan perbaikan untuk Anki dan add-on terbaru dilanjutkan di fork arbyste.

=== "Gelap: depan"

    ![Depan kartu jp-mining-note, tema gelap](https://aquafina-water-bottle.github.io/jp-mining-note/assets/fushinnsha/dark_front.png){ loading=lazy }

=== "Gelap: belakang"

    ![Belakang kartu jp-mining-note, tema gelap](https://aquafina-water-bottle.github.io/jp-mining-note/assets/fushinnsha/dark_back.png){ loading=lazy }

=== "Terang: depan"

    ![Depan kartu jp-mining-note, tema terang](https://aquafina-water-bottle.github.io/jp-mining-note/assets/fushinnsha/light_front.png){ loading=lazy }

=== "Terang: belakang"

    ![Belakang kartu jp-mining-note, tema terang](https://aquafina-water-bottle.github.io/jp-mining-note/assets/fushinnsha/light_back.png){ loading=lazy }

### Crop Theft

| | |
|---|---|
| Situs | [GitHub](https://github.com/Kuuuube/crop-theft) |
| Unduh | [Crop Theft Vocab.apkg](https://raw.githubusercontent.com/Kuuuube/crop-theft/main/crop_theft_vocab/Crop%20Theft%20Vocab.apkg) |

Note type kosakata yang minimalis tapi lengkap, buatan Kuuube. Repositorinya juga berisi panduan pengaturan Yomitan, cek kartu duplikat, dan mengurutkan kartu berdasarkan frekuensi.

=== "Depan"

    ![Depan kartu Crop Theft](https://raw.githubusercontent.com/Kuuuube/crop-theft/main/crop_theft_vocab/images/crop_theft_vocab_front.png){ loading=lazy }

=== "Belakang"

    ![Belakang kartu Crop Theft](https://raw.githubusercontent.com/Kuuuube/crop-theft/main/crop_theft_vocab/images/crop_theft_vocab_back.png){ loading=lazy }

### Vertical Cards

| | |
|---|---|
| Situs | [GitHub](https://github.com/kiwakiwaa/vertical-cards) |
| Unduh | [Rilis terbaru](https://github.com/kiwakiwaa/vertical-cards/releases) |

Note type dengan tulisan vertikal (縦書き) yang dirancang untuk kamus Yomitan. Di HP atau jendela sempit, tampilannya otomatis berubah jadi mendatar. Definisi dan gambar bisa digilir, dan beberapa kamus bisa dilipat.

=== "PC"

    ![Demo Vertical Cards di PC](https://raw.githubusercontent.com/kiwakiwaa/vertical-cards/main/assets/desktop-demo.gif){ loading=lazy }

=== "HP"

    ![Tampilan Vertical Cards di HP](https://raw.githubusercontent.com/kiwakiwaa/vertical-cards/main/assets/mobile.jpg){ loading=lazy width=360 }

### Japanese Tategaki Note Type

| | |
|---|---|
| Situs | [AnkiWeb](https://ankiweb.net/shared/info/1629919024) (cara setup ada di deskripsinya) |
| Unduh | [AnkiWeb](https://ankiweb.net/shared/info/1629919024) |

Note type tulisan vertikal buatan IMMERSION JUNKIES, cocok untuk masa transisi ke kamus monolingual. Desainnya diambil dari note type Matt vs Japan, lalu ditambah mode malam dan mode HP. Deskripsi di AnkiWeb menjelaskan pengaturan Yomitan untuk mining satu klik.

=== "PC: terang"

    ![Japanese Tategaki Note Type di PC, tema terang](https://i.imgur.com/KJXlqVw.png){ loading=lazy }

=== "PC: malam"

    ![Japanese Tategaki Note Type di PC, mode malam](https://i.imgur.com/TJflH8L.png){ loading=lazy }

=== "HP"

    ![Japanese Tategaki Note Type di HP](https://i.imgur.com/ZstO2HS.png){ loading=lazy width=300 }

=== "HP: malam"

    ![Japanese Tategaki Note Type di HP, mode malam](https://i.imgur.com/GRwt3hi.png){ loading=lazy width=300 }

### mj note type

| | |
|---|---|
| Situs | [GitHub](https://github.com/watchtheflowers/mj-s-note-type) |
| Unduh | [Versi biasa](https://github.com/watchtheflowers/mj-s-note-type/releases/download/standard/mj.auto.mining.apkg) · [Versi donut](https://github.com/watchtheflowers/mj-s-note-type/releases/download/standard/mj.donut.mining.apkg) |

Note type mining yang bersih dan ringan, dikembangkan dari template Tigy01. Ada kanji hover, daftar frekuensi, info sumber, grafik pitch accent, dan tampil baik di AnkiMobile maupun AnkiDroid. Versi *donut* adalah variasi tampilannya.

=== "Biasa"

    ![Kartu mj note type versi biasa](https://github.com/user-attachments/assets/6f67938f-caa4-4424-b772-ac758f96410e){ loading=lazy width=420 }

=== "Donut"

    ![Kartu mj note type versi donut](https://github.com/user-attachments/assets/f6337f48-6fb0-45f0-b593-7d76e1df13fa){ loading=lazy width=420 }

### Clean Anki Cards

| | |
|---|---|
| Situs | [GitHub](https://github.com/Michael-128/clean-anki-cards) |
| Unduh | [Template kartu kosakata](https://github.com/Michael-128/clean-anki-cards/blob/main/Vocab/vocab-template.md) (salin ke note type kamu) |

Template kartu yang bersih untuk mining kosakata dan latihan menulis. Template-nya disalin manual ke `Cards` di Anki, bukan diimpor dari berkas `.apkg`.

=== "Contoh 1"

    ![Contoh kartu Clean Anki Cards](https://github.com/Michael-128/clean-anki-cards/assets/116978510/24d59a88-0ccf-4cf5-9807-027126cea382){ loading=lazy width=420 }

=== "Contoh 2"

    ![Contoh kartu Clean Anki Cards, kartu lain](https://github.com/Michael-128/clean-anki-cards/assets/116978510/d1b20d59-8fcf-4925-8bd8-67117d07c8c5){ loading=lazy width=420 }

### Lapis Themes

| | |
|---|---|
| Situs | [GitHub](https://github.com/ccos89/lapis-themes) |
| Unduh | Salin CSS tema dari repositorinya ke `Styling` Lapis |

Bukan note type baru, melainkan warna alternatif untuk Lapis: Rosé Pine, Gruvbox, Catppuccin, Cyberpunk, dan lainnya. Cocok kalau kamu sudah memakai Lapis tapi ingin tampilan lain. Tema ini dibuat untuk Lapis v1.6.0 dan bisa merusak tampilan kartu di versi Lapis lain, jadi cek dulu versinya. Simpan juga `Styling` lamamu, karena [memperbarui Lapis](pembaruan-note-type.md) akan mengembalikannya ke bawaan.

=== "Rosé Pine"

    ![Lapis dengan tema Rosé Pine](https://raw.githubusercontent.com/ccos89/lapis-themes/master/img/rose_pine.png){ loading=lazy }

=== "Catppuccin Mocha"

    ![Lapis dengan tema Catppuccin Mocha](https://raw.githubusercontent.com/ccos89/lapis-themes/master/img/catppuccin-mocha.png){ loading=lazy }

=== "Gruvbox Dark"

    ![Lapis dengan tema Gruvbox Dark](https://raw.githubusercontent.com/ccos89/lapis-themes/master/img/gruvbox-dark.png){ loading=lazy }

=== "Gruvbox Light"

    ![Lapis dengan tema Gruvbox Light](https://raw.githubusercontent.com/ccos89/lapis-themes/master/img/gruvbox-light.png){ loading=lazy }

---

## Note Type Lama

Note type di bawah ini dibuat sebelum Yomitan menggantikan Yomichan. Banyak note type modern, termasuk Lapis, dikembangkan dari sini.

### Anime Cards (Basic Mining Deck)

| | |
|---|---|
| Situs | [GitHub](https://github.com/friedrich-de/Basic-Mining-Deck) · [AnimeCards](https://animecards.site/ankicards/) |
| Unduh | [AnkiWeb](https://ankiweb.net/shared/info/151553357) |

Note type klasik dari AnimeCards: kata di depan, lalu bacaan, arti, audio, dan kalimat di belakang. Repositorinya sudah diarsipkan sejak Maret 2025, dan pembuatnya menyarankan pindah ke Lapis.

=== "Contoh dek"

    ![Contoh kartu Basic Mining Deck](https://raw.githubusercontent.com/friedrich-de/Basic-Mining-Deck/master/sample_image.png){ loading=lazy }

=== "Kartu dari anime"

    ![Contoh kartu anime dari AnimeCards](https://animecards.site/images/lapis_modified_2.png){ loading=lazy }

### Tatsumoto's TSC

| | |
|---|---|
| Situs | [Penjelasan TSC](https://tatsumoto.neocities.org/blog/discussing-various-card-templates.html#targeted-sentence-cards-or-mpvacious-cards) |
| Unduh | [AnkiWeb](https://ankiweb.net/shared/info/1557722832) |

*Targeted sentence card*: kalimat lengkap di depan dengan satu kata sasaran yang disorot, arti dan audio di belakang. jp-mining-note awalnya dikembangkan dari note type ini. Varian buatan pengguna lain ada di [AJATT-Tools AnkiNoteTypes](https://github.com/Ajatt-Tools/AnkiNoteTypes).

![Contoh targeted sentence card](https://tatsumoto.neocities.org/blog/img/example-mpvacious-card.webp){ loading=lazy }

### Eminent Note Type

| | |
|---|---|
| Situs | [cademcniven.com](https://cademcniven.com/projects/notetype2/) |
| Unduh | [GitHub (V2.4)](https://github.com/cademcniven/cademcniven.com-dev/releases/tag/V2.4) |

Note type sentence mining buatan Cade: kanji bisa diarahkan kursor, audio kata dan kalimat, furigana dengan tanda turunnya pitch, blur gambar NSFW, dan urutan kartu berdasarkan frekuensi. Sebagian fitur butuh pengaturan Yomichan dari pembuatnya.

=== "Depan"

    ![Depan kartu Eminent Note Type](https://cademcniven.com/images/card_front-M4BXXShqiw-750w.jpeg){ loading=lazy }

=== "Belakang"

    ![Belakang kartu Eminent Note Type](https://cademcniven.com/images/card_back-xbXcF4wXEl-750w.jpeg){ loading=lazy }

### Anacreon's Template

| | |
|---|---|
| Situs | [Anacreon DJT](https://anacreondjt.gitlab.io/docs/anki_css/) |
| Unduh | Salin template dan CSS dari halamannya |

Template dan CSS untuk Anime Cards. Di PC, gambar di kiri dan arti di kanan. Di HP, keduanya bertumpuk.

![Kartu dengan CSS Anacreon](https://anacreondjt.gitlab.io/img/with_css.png){ loading=lazy }

### Klieret's Templates

| | |
|---|---|
| Situs | [GitHub](https://github.com/klieret/anki-card-templates) |
| Unduh | [ZIP](https://github.com/klieret/anki-card-templates/archive/master.zip) |

Template untuk kartu kanji dan kosakata. Kartu hanya dibuat kalau ada pasangan soal-jawaban yang masuk akal, dan ada deretan tombol untuk mencari kata di kamus, kanji.koohii, dan Google Images.

![Tampilan Klieret's Templates di HP](https://raw.githubusercontent.com/klieret/readme-files/master/anki-card-templates/phone.png){ loading=lazy width=360 }

---

## Template Umum

Template ini tidak khusus untuk bahasa Jepang, tapi bisa jadi inspirasi kalau kamu ingin mengubah tampilan kartu sendiri:

- [Prettify](https://github.com/pranavdeshai/anki-prettify)
- [Modern Card Themes](https://github.com/b3nj5m1n/moderncardthemes)
- [Anki Minimal Language Learning Template](https://github.com/chaosarium/anki-minimal-language-learning-template)
- [Anki Cards Templates SuperList](https://github.com/Troyciv/anki-templates-superlist)
