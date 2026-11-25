---
description: "Catatan perubahan situs Philia Space: halaman baru, pembaruan panduan, dan perbaikan."
hide:
  - footer
---
# Riwayat Perubahan

??? question "Keterangan<small>(click here)</small>"

    - Penambahan = Penambahan halaman baru

    - Pembaruan = Pembaruan halaman tutorial atau pengaturan yang sudah ada ke versi terbaru

    - Perbaikan = Memperbaiki kesalahan apapun dari halaman yang sudah ada

    - Untuk Penulis = Aturan atau konvensi baru untuk yang ikut menulis dan menyunting panduan

---

## 2026

---

### November

**25-11-2026**

*Lisensi dan kredit TheMoeWay*

- Perbaikan
       - Terjemahan dari TheMoeWay sekarang berlisensi GPL-3.0, sama dengan versi aslinya. Sebelumnya tertulis CC BY-SA 4.0, dan itu keliru karena terjemahan karya GPL-3.0 wajib tetap memakai GPL-3.0
       - Kredit ke TheMoeWay dan penulisnya, shoui, sekarang selalu terlihat di bagian atas [Panduan Bahasa Jepang](panduan.md), [30 Hari Awal](rutinitas-awal.md), [Belajar Kanji](kanji.md), [Perbaiki Font](font.md), dan [Mengetik Bahasa Jepang](ime.md), tanpa perlu diklik dulu
       - Kredit ke LazyGuide di [Panduan Ringkas Bahasa Jepang](panduan-ringkas-JP.md) juga sekarang selalu terlihat
- Untuk Penulis
       - Kotak kredit untuk halaman terjemahan TheMoeWay di PANDUAN-GAYA diganti ke versi yang selalu terlihat dan menyebut penulis serta lisensinya

*Kredit LazyGuide*

- Perbaikan
       - Semua halaman dari LazyGuide sekarang punya kotak kredit di bagian atas yang menyebut halaman aslinya, penulisnya (LazyGuideJP), dan lisensinya. Kotaknya dibedakan antara terjemahan, adaptasi, dan yang hanya sebagian diambil dari LazyGuide
       - [Mining Manga di Android](setup-manga-android-lazy-guide.md), [Mining Anime di PC](setup-anime-pc-lazy-guide.md), dan [Memperbarui Note Type](pembaruan-note-type.md) sebelumnya belum menyebut LazyGuide sama sekali
       - [Beranda](index.md) sekarang menyebut lisensi teks GPL-3.0, bukan lagi CC BY-SA 4.0
- Untuk Penulis
       - PANDUAN-GAYA sekarang punya kotak kredit untuk halaman dari LazyGuide, beserta cara memilih antara terjemahan, adaptasi, atau sebagian

*Note type dan sumber dari jp-mining-note*

- Penambahan
       - Halaman baru [Pilihan Note Type](note-type.md): daftar note type untuk mining, lengkap dengan gambar atau video contoh dari pembuatnya masing-masing, termasuk beberapa note type yang dibagikan di server TheMoeWay. Daftar note type di [Sumber Belajar](sumber/index.md) dipindah ke sini
       - Halaman baru [Pindah ke jp-mining-note](pindah-ke-jp-mining-note.md): cara memindahkan kartu dari Lapis, Mining-JP, Anime Cards, dan note type lain ke jp-mining-note tanpa kehilangan jadwal ulasan
- Pembaruan
       - [Sumber Belajar](sumber/index.md) sekarang juga mengambil dari JP Resources milik jp-mining-note: bacaan tentang Anki, beberapa add-on baru, tips tampilan Yomitan, serta skrip ShareX dan Anki
       - [Setup Anki PC](setup-anki-pc-lazy-guide.md) punya daftar bacaan lanjutan tentang Anki

*Daftar isi di kanan halaman*

- Pembaruan
       - Daftar isi di kanan halaman sekarang dikelompokkan per bagian: judul bagian ditebalkan dan dipisah garis tipis, subbagian berderet di sepanjang garis di bawahnya, dan posisi bacaanmu ditandai warna biru

*Sumber Belajar dipecah per kategori*

- Pembaruan
       - Sumber Belajar sekarang punya halaman [Ringkasan](sumber/index.md) dan empat halaman per kategori: [Bahasa](sumber/bahasa.md), [Software](sumber/software.md), [Immersion](sumber/immersion.md), dan [Ujian & Kerja](sumber/ujian.md). Susunannya mengikuti Wotaku
       - Isi tiap bagian sekarang berupa tabel bertab. Tabel software punya kolom platform dengan ikon Linux, Windows, macOS, Android, iOS, web, dan ekstensi browser, jadi kamu bisa langsung melihat alat mana yang jalan di perangkatmu
       - Sumber yang paling direkomendasikan ditandai bintang, bukan lagi huruf tebal
       - Alamat lama Sumber Belajar otomatis dialihkan ke halaman Ringkasan
       - Di HP, tiap baris di halaman Sumber Belajar tampil sebagai kartu kecil, jadi keterangannya terbaca utuh tanpa digeser ke samping. Keterangan ikon juga tersusun rapi sebagai daftar
       - Bagian Semua-dalam-Satu di halaman [Software](sumber/software.md) punya tab Disarankan berisi Manatan dan Fushi, supaya pemula langsung tahu harus mulai dari mana
       - Ikon platform sekarang bisa dibacakan pembaca layar, urutannya selalu sama, dan platform yang masih beta ditulis jelas dengan label "beta:"
       - Di layar besar, teks dan tabel di seluruh situs tidak lagi ikut membesar, jadi lebih banyak isi muat dalam satu layar. Tabel juga dibuat lebih rapat, dan semua halaman memakai kolom isi yang lebih lebar di layar besar
- Penambahan
       - Puluhan alat baru dari kanal #resources-sharing TheMoeWay masuk ke halaman [Software](sumber/software.md), misalnya Fushi, Hoshi Reader Desktop, MacPopup, OwOtan, Hachidori, Kimochi, meikipop, Yomipv, SubMiner, MaruReader, dan Yomihon
       - Tab baru "Pilihan Cepat per Perangkat" di halaman [Software](sumber/software.md) merangkum alat yang disarankan untuk Android, iOS, Windows, macOS, dan Linux
- Untuk Penulis
       - Isi halaman Sumber Belajar sekarang ditulis sebagai daftar HTML (`ps-tabel`), bukan tabel Markdown, supaya tampil rapi sebagai kolom di komputer dan sebagai kartu di HP. Tab di halaman itu memakai format `/// tab | Judul`. Contoh dan aturannya ada di PANDUAN-GAYA, bagian Halaman Sumber Belajar
       - Ikon platform ditulis dengan kode ikon Material yang diberi nama, misalnya `:simple-linux:{ title="Linux" role="img" aria-label="Linux" }`. Daftar ikon yang dipakai ada di bagian Keterangan ikon di halaman [Ringkasan](sumber/index.md#keterangan-ikon)

**24-11-2026**

*Tampilan baru beranda*

- Pembaruan
       - [Beranda](index.md) disusun ulang dengan identitas visual baru: kamu bisa memilih titik mulai (baru mulai, siap mining, atau sudah jalan) dan memilih panduan menurut media yang kamu tonton atau baca, lalu menurut perangkatnya
       - Halaman Mengetik Bahasa Jepang, isian note type, Fushi, Hoshi Reader Android, dan Sumber Belajar sekarang bisa dibuka langsung dari beranda
       - Header di mode terang sekarang putih dengan teks gelap
- Perbaikan
       - Mode gelap memakai abu-abu sangat gelap dan teks yang sedikit diredupkan supaya lebih nyaman dibaca, dan teks redup yang sebelumnya terlalu samar sekarang lebih jelas

**23-11-2026**

*Panduan font Linux langkah demi langkah*

- Pembaruan
       - Bagian Linux di [Perbaiki Font](font.md) sekarang berisi perintah siap salin untuk Ubuntu dan Arch, file aturan fontconfig yang sudah jadi, cara memeriksa hasilnya dengan `fc-match`, dan cara membatalkannya
       - Locale Jepang dipindah ke bagian opsional karena tidak wajib untuk memperbaiki font
       - Pengaturan `Fixed-width font` ditambahkan di bagian Chromium

*Halaman baru: Mengetik Bahasa Jepang*

- Penambahan
       - [Mengetik Bahasa Jepang](ime.md): cara memasang dan memakai keyboard Jepang (IME), adaptasi dari TheMoeWay. Versi aslinya hanya untuk Windows, di sini ditambah macOS dan Linux (Mozc), latihan mengetik, dan daftar tombol untuk ketiga sistem
- Perbaikan
       - Langkah memasang keyboard Jepang di [30 Hari Awal](rutinitas-awal.md) dan [Belajar Kanji](kanji.md) sekarang menautkan halaman itu

*Sumber belajar visa Gijinkoku*

- Penambahan
       - [Sumber Belajar](sumber/ujian.md#gijinkoku): bagian baru untuk visa Gijinkoku (技人国), berisi syarat resmi, aturan bahasa yang berlaku sejak 15 April 2026, dan situs untuk mencari kerja. Sebagian tautan dikumpulkan dari server Philia Space, KaburAjaDulu, dan TheMoeWay
- Perbaikan
       - Tautan OTIT dan program magang Kemnaker di bagian SSW diberi keterangan bahwa keduanya untuk program magang (Ginou Jisshuu)

**18-11-2026**

*Judul halaman lebih jelas di mesin pencari*

- Perbaikan
       - 20 halaman diberi judul tab dan judul di hasil pencarian yang lebih jelas, misalnya "Mining Anime di Android" alih-alih "Anime". Nama di menu tetap sama
       - 6 halaman LazyGuide diberi deskripsi sendiri, dan 12 gambar di [Perbaiki Font](font.md) dan [Setup Yomitan dan Anki](setup-yomitan-pc.md) diberi teks alternatif
       - Tautan ke LazyGuide dipindah dari judul halaman ke baris "Diadaptasi dari LazyGuide" tepat di bawahnya
       - Baris "Diunggah · Diperbarui" di atas halaman diganti dengan tanggal dibuat dan terakhir diperbarui di bawah halaman, yang terisi otomatis setiap ada perubahan
       - Halaman Tentang Retention yang masih kosong dihapus, begitu juga bagian yang menautkannya di [Setup Anki di PC](setup-anki-pc-lazy-guide.md)
       - Alamat lama Memperbarui: Format Lapis sekarang langsung dialihkan ke [Memperbarui Note Type](pembaruan-note-type.md)
- Untuk Penulis
       - Penanda `upstream` di halaman LazyGuide sekarang boleh berada tepat setelah front matter
       - Tanggal halaman tidak perlu ditulis manual lagi

*Cadangan Anki Deck Soal JLPT*

- Perbaikan
       - Tautan unduhan Anki Deck Soal JLPT 2010–2025 di thread Discord sudah mati, jadi [Proyek Komunitas, Rute 2](proyek.md#rute-2-bahasa-untuk-tes-jlpt-jft) sekarang menautkan cadangan dari anggota, dengan catatan bahwa soal listening-nya tidak bisa dipakai

**17-11-2026**

*Bahan ujian JLPT, JFT, SSW, dan tes lainnya*

- Pembaruan
       - [Sumber Belajar](sumber/ujian.md#jlpt): bagian JLPT ditambah info resmi, arsip soal tahun lalu, dan situs simulasi
- Penambahan
       - [Sumber Belajar](sumber/ujian.md#jft): bagian JFT berisi situs resmi, simulasi ujian, kisi-kisi, dan modul
       - [Sumber Belajar](sumber/ujian.md#ssw-tokutei-ginou): bagian SSW berisi materi resmi per bidang, modul, kisi-kisi, dan daftar resmi untuk cek LPK dan TSK sebelum mendaftar
       - [Sumber Belajar](sumber/ujian.md#tes-jepang-lainnya): bagian baru untuk NAT-TEST, J.TEST, BJT, J-CAT, Kanken, EJU, dan kaigo, lengkap dengan contoh soal resmi dan buku teks kaigo berbahasa Indonesia

*Format Riwayat Perubahan*

- Pembaruan
       - Perubahan di tanggal yang sama sekarang dikumpulkan di bawah satu tanggal, diurutkan dari yang paling awal sampai yang paling baru
- Untuk Penulis
       - Perubahan baru di tanggal yang sudah ada ditulis di bawah perubahan terakhir tanggal itu, dengan judul miring, bukan sebagai tanggal baru

*Dek Ankidrone pindah ke rute JLPT*

- Perbaikan
       - [Proyek Komunitas](proyek.md#rute-2-bahasa-untuk-tes-jlpt-jft): Ankidrone Essentials V9 dari RenRen dan Ankidrone Essentials V1 dari Jibal dipindah dari rute bahasa untuk diri sendiri ke rute tes, karena keduanya dek kosakata JLPT dari buku JLPT Tango
       - [Proyek Komunitas](proyek.md#rute-2-bahasa-untuk-tes-jlpt-jft): keterangan dek Jibal dibetulkan, isinya sudah N5 dan N4, bukan hanya N5
       - [Proyek Komunitas](proyek.md#kendala-yang-diketahui): tautan Kaishi V2 ternyata masih berlaku, jadi kendala unduhannya diganti dengan cara membukanya di Chrome atau browser lain
- Penambahan
       - [Proyek Komunitas](proyek.md#rute-2-bahasa-untuk-tes-jlpt-jft): Multilingual Eggrolls JLPT 10k, yang di rekomendasi Discord disebut pilihan utama untuk JLPT

**16-11-2026**

*Dek Anki komunitas di halaman Proyek Komunitas*

- Penambahan
       - [Proyek Komunitas](proyek.md#dek-anki-komunitas): bagian baru berisi dek Anki buatan anggota, terutama yang masih dirawat RenRen, Raychi, dan Jibal, lengkap dengan status dan tanggal pembaruan terakhir
       - [Proyek Komunitas](proyek.md#dek-anki-komunitas): dek dikelompokkan dalam empat rute: bahasa untuk diri sendiri, untuk tes, untuk kerja, dan untuk lanjut pendidikan
       - [Proyek Komunitas](proyek.md#kendala-yang-diketahui): kendala dek yang sudah dilaporkan beserta cara mengatasinya, misalnya kartu kosong di HP pada Kotoba Deck
       - [Proyek Komunitas](proyek.md#kendala-yang-diketahui): cara mengunduh dek dan kamus dari Google Drive di HP kalau muncul "Jenis file ini tidak didukung" (Android) atau "Pratinjau tidak tersedia" (iPhone), lalu cara mengimpornya ke Anki, Yomitan, Hoshi Reader, atau Manatan, serta saran mencoba browser lain, lalu ganti DNS atau pakai VPN, kalau tautannya tidak bisa dibuka
       - [Proyek Komunitas](proyek.md#riwayat-pembaruan): riwayat pembaruan dek per pembuat, dengan tautan ke pengumumannya di Discord
       - [Proyek Komunitas](proyek.md#rhdict): RHDict, kamus Jepang-Indonesia format Yomitan
       - [Proyek Komunitas](proyek.md#alat-belajar-lainnya) dan [Sumber Belajar](sumber/index.md): PhiList, alat untuk mengecek tingkat kesulitan bahasa Jepang anime, manga, novel, dan media lain
- Pembaruan
       - [Proyek Komunitas](proyek.md#alat-belajar-lainnya) dan [Sumber Belajar](sumber/index.md): Tes Frekuensi Kosakata diganti Philia Test versi baru, tes untuk mengecek berapa banyak kanji yang bisa kamu baca
       - [Setup Anki PC](setup-anki-pc-lazy-guide.md#tip-4-dek-anki-dari-komunitas): tip baru yang mengarahkan ke Dek Anki Komunitas, dengan tautan ke tiap rute dan ke daftar kendala
       - [Panduan Bahasa Jepang](panduan.md#24-belajar-kosakata-dengan-anki), [Panduan Ringkas](panduan-ringkas-JP.md), dan [30 Hari Awal](rutinitas-awal.md): tautan ke Dek Anki Komunitas di bawah daftar dek kosakata

*Pratinjau tautan di Discord dan media sosial*

- Penambahan
       - Setiap halaman sekarang punya kartu pratinjau sendiri berisi judul dan deskripsi halaman, jadi tautan yang dibagikan di Discord, WhatsApp, atau media sosial tampil sebagai kotak bergambar
       - Halaman di bawah menu PC, Android, dan iOS diberi nama perangkatnya di kartu, misalnya "Anki (PC)"
- Untuk Penulis
       - Kartu dibuat otomatis saat build oleh plugin `social` dengan layout `layouts/philia.yml`. Deskripsi kartu diambil dari `description:` di bagian atas halaman, dan halaman tanpa deskripsi memakai deskripsi situs
       - Plugin ini butuh Cairo. Untuk mengedit teks tanpa Cairo, jalankan `KARTU_SOSIAL=false mkdocs serve`

*Tautan mati di Sumber Belajar*

- Perbaikan
       - [Sumber Belajar](sumber/index.md): tautan yang sudah mati dibuang, antara lain VNCR, OJAD, Fuseji, BilingualManga, mangareader.to, Todaii, CDRomance, Misuzu, HoriSan, Japanese Live TV, korpus BCCWJ dan NWJC, serta situs Yuzu dan Citron yang tidak bisa dibuka lagi
       - [Sumber Belajar](sumber/index.md): Master reference grammar, DOJG Deck, dan NeeView diarahkan ke alamat yang masih hidup

**11-11-2026**

*Hoshi Reader Android masuk menu*

- Pembaruan
       - Menu **Setup Mining** sekarang punya kelompok **Android** berisi [LN & Buku](Setup-Hoshi-Reader.md), yaitu panduan Hoshi Reader untuk membaca light novel dan buku di HP Android

*Audiobook di Manatan*

- Perbaikan
       - [Novel (EPUB) di Manatan](Setup-Manatan-novels.md#audiobook): catatan bahwa audiobook belum didukung ternyata keliru dan sudah diganti dengan langkah memutar audiobook bersamaan dengan bukunya, lengkap dengan screenshot tiap langkah; fitur ini hanya ada di aplikasi versi sekarang, bukan di versi lama yang dibuka lewat browser
       - [Novel (EPUB) di Manatan](Setup-Manatan-novels.md#impor-buku): langkah impor buku disesuaikan dengan aplikasi versi sekarang (ikon `+` di halaman `Novel`), screenshot-nya diganti

*Pemutar video, popup kamus, dan flashcard Manatan*

- Pembaruan
       - [Setup Manatan](Setup-Manatan.md#anime): gambar dan daftar tombol pemutar video diganti mengikuti aplikasi versi sekarang, termasuk tombol baru untuk trek audio, daftar kalimat subtitle, dan statistik kosakata
       - [Setup Manatan](Setup-Manatan.md#pengaturan-popup-dictionary): pengaturan popup kamus ditulis ulang mengikuti tampilan baru, dengan penjelasan pengaturan yang paling sering diubah
       - [Setup Manatan](Setup-Manatan.md#info-2-custom-popup-css): Custom Popup CSS sekarang satu untuk video, manga, dan novel, tidak lagi terpisah
       - [Setup Manatan](Setup-Manatan.md#tips-1-media-dalam-bahasa-lain): catatan bahwa popup kamus untuk bahasa lain butuh profil tambahan (membership), karena versi gratis hanya punya satu profil
- Penambahan
       - [Pengaturan Note Type](pengaturan-note-type.md): halaman baru berisi isian field kartu Anki untuk Lapis, Kiku, Senren, dan Mining-JP, dalam versi Yomitan dan Manatan, termasuk pengaturan kartu duplikat dan cara Senren menyimpan banyak adegan dalam satu kartu; ada di menu **Setup Mining**
- Perbaikan
       - [Setup Manatan](Setup-Manatan.md#info-tambahan-dan-tips): tips penguraian kosakata dihapus karena hanya berlaku untuk Yomitan, bukan popup kamus Manatan

*Pengaturan Senren di Manatan*

- Perbaikan
       - [Pengaturan Note Type](pengaturan-note-type.md#isian-per-note-type): isian Senren untuk Manatan diganti dengan pengaturan yang sudah dicoba dan berhasil menggabungkan beberapa adegan ke satu kartu, dengan cara pembaruan field Yomitan dan Manatan ditulis terpisah

*Tabel dan tampilan lebih mudah dibaca*

- Perbaikan
       - Tabel lebar di semua halaman tidak lagi memotong isinya huruf per huruf. Tabel yang lebih lebar dari layar bisa digeser ke samping (geser jari di HP, Shift + scroll atau trackpad di PC), dan kolom pertamanya tetap terlihat saat digeser
       - [Pengaturan Note Type](pengaturan-note-type.md#isian-per-note-type): tabel Senren dipecah jadi tab Yomitan dan Manatan, dan kolom cara pembaruan field dipindah ke depan supaya tidak terlewat
       - Tautan, tulisan di bagian atas halaman, dan tombol "Sebelumnya/Berikutnya" di bawah halaman dibuat lebih mudah dibaca
       - Tautan di dalam teks sekarang bergaris bawah, dan tombol di bagian atas halaman lebih mudah ditekan di HP

*Teks beranda*

- Perbaikan
       - [Beranda](index.md): beberapa keterangan yang keliru diperbaiki, misalnya biaya situs (yang dibayar hanya domain), isi halaman Panduan, dan permintaan sebelum bertanya di Discord
       - [Beranda](index.md): keterangan lisensi dilengkapi, isi panduan boleh disalin dan diubah dengan menyebut sumber dan memakai lisensi yang sama (CC BY-SA 4.0)
       - [Beranda](index.md): tulisan kecil di bagian paling bawah lebih mudah dibaca

**10-11-2026**

*Anime dan manga dari ekstensi di Manatan*

- Pembaruan
       - [Setup Manatan](Setup-Manatan.md#penggunaan-media): ada langkah mencari judul dari ekstensi dan menyimpannya ke Library, lewat pencarian global untuk manga dan per sumber untuk anime
       - [Setup Manatan](Setup-Manatan.md#ekstensi-anime-yang-sudah-dicoba): daftar ekstensi anime yang sudah dicoba, lengkap dengan bahasa dan jenis subtitlenya, menggantikan rekomendasi lama di Pertanyaan Umum
       - [Setup Manatan](Setup-Manatan.md#anime): screenshot pemutar video diganti mengikuti tampilan baru, ada langkah memasang subtitle Jimaku langsung dari pemutar, dan fungsi tiap tombol dijelaskan per nomor
       - [Setup Manatan](Setup-Manatan.md#manga): screenshot pengaturan pembaca manga diganti mengikuti tampilan baru, ditambah cara membuka pengaturannya, saran mode baca kanan ke kiri untuk manga Jepang, dan penjelasan singkat tiap tab
       - [Novel (EPUB) di Manatan](Setup-Manatan-novels.md): cara impor diperbarui (menu tiga titik di `Novels`, bisa EPUB, PDF, atau TXT), ada catatan konversi file `.azw3`, screenshot pembaca dan pengaturannya, serta catatan bahwa audiobook belum didukung, dengan tautan ke Yatsu Whispersync (PC) dan Hoshi Reader (Android dan iPhone) sebagai gantinya
       - [Setup Manatan](Setup-Manatan.md#tips-2-mode-putar-dan-shortcut-pemutar-video): tips baru tentang mode putar (misalnya jeda otomatis tiap kalimat) dan shortcut keyboard pemutar video

*Screenshot Hoshi Reader Android*

- Pembaruan
       - [Setup Hoshi Reader (Android)](Setup-Hoshi-Reader.md): screenshot dari HP untuk setiap langkah, dan langkah disesuaikan dengan versi 1.5.0 (impor buku lewat tombol `+`, format kartu Anki, letak audio lokal, tombol volume yang perlu dinyalakan dulu)
       - [Setup Hoshi Reader (Android)](Setup-Hoshi-Reader.md#info-2-audiobook): langkah memutar audiobook dengan Sasayaki, termasuk cara mencocokkan audio tanpa file subtitle
       - [Setup Hoshi Reader (Android)](Setup-Hoshi-Reader.md#membaca-dan-mining): penjelasan menu di dalam pembaca, cara mengelola buku dan rak, statistik membaca, dan cara memperbarui aplikasi
       - [Setup Hoshi Reader (Android)](Setup-Hoshi-Reader.md#info-4-pilihan-sumber-audio): pilihan sumber audio untuk HP dengan memori terbatas, yaitu versi ringan sekitar 2 GB dan versi online tanpa unduhan

**08-11-2026**

*Subtitle Jimaku di asbplayer*

- Pembaruan
       - [Setup Mining Anime di PC](setup-anime-pc-lazy-guide.md#langkah-langkah-penggunaan-video-streaming): ekstensi animetan diganti ke asbplayer resmi, yang sekarang sudah bisa mencari subtitle Jimaku sendiri, lengkap dengan langkah dan screenshot barunya

**06-11-2026**

*Hoshi Reader untuk iPhone*

- Penambahan
       - [Setup Hoshi Reader (iOS)](Setup-Hoshi-Reader-iOS.md): membaca light novel dan buku di iPhone atau iPad, dari pasang aplikasi, kamus, kartu Anki lewat AnkiMobile atau AnkiConnect, audio lokal, sampai audiobook, lengkap dengan tips, pertanyaan umum, dan masalah umum
       - [Proyek Komunitas](proyek.md#jidict-frequency): JIDict Frequency, kamus frekuensi Jepang-Indonesia untuk Yomitan dengan 13.168 kosakata N1–N5
- Pembaruan
       - Menu mining dipisah jadi dua: **LazyGuide - Mining** untuk halaman adaptasi LazyGuide, dan **Setup Mining** untuk panduan buatan Philia Space
       - Kedua menu itu sekarang dikelompokkan per perangkat: PC, Android, dan iOS
       - Menu "Anime Desktop" sekarang bernama "Anime PC"
       - [Setup Mining Anime di PC](setup-anime-pc-lazy-guide.md) tidak lagi berlabel MacOS, karena langkahnya berlaku untuk semua PC
       - [Belajar Kanji](kanji.md) ditulis ulang agar lebih santai, dengan tabel ringkasan di awal
       - [Perbaiki Font](font.md) ditulis ulang dan disamakan dengan TheMoeWay terbaru: langkah Windows 11 dengan dua pilihan cara, langkah macOS terbaru, dan tips nama file font di Anki supaya tidak terhapus

*Audiobook di Yatsu Reader*

- Pembaruan
       - [LN & Buku PC](setup-LN-pc-lazy-guide.md#info-3-audiobook-dengan-yatsu-whispersync): cara membaca sambil mendengarkan audiobook di Yatsu Reader dengan Yatsu Whispersync

*Sumber Belajar*

- Penambahan
       - [Sumber Belajar](sumber/index.md): kumpulan tautan alat dan bahan belajar bahasa Jepang dari kuri, TheMoeWay, Ten, dan Wotaku, dikelompokkan per topik dengan deskripsi bahasa Indonesia
       - [Rekomendasi Add-on Anki](sumber/software.md#add-on-anki): daftar add-on pilihan Philia Space beserta fungsi dan kode pasangnya
       - [JIDict Web](sumber/software.md#yomitan-dan-kamus) di daftar kamus, lengkap dengan cara memasangnya di Android dan iOS
- Pembaruan
       - Menu **Sumber Belajar** ditambahkan di navigasi, di atas **Proyek Komunitas**
- Perbaikan
       - [Setup Fushi](Setup-Fushi.md#sumber-online-manga-anime-novel): tautan toko manga Keiyoushi diperbarui, dan ada cara menambah sumber web novel (Syosetsu dan Kakuyomu) lewat toko LNReader
       - [Setup Manatan](Setup-Manatan.md#pasang-ekstensi): daftar repositori ekstensi diperbarui; tautan Keiyoushi diganti, repositori yang sudah mati (Yuzono manga, Kohi-den, Skittyblock) dihapus, Yuzono sekarang jadi rekomendasi untuk anime, dan ada tambahan repositori Amqx untuk manga

**05-11-2026**

*Setup Fushi*

- Penambahan
       - Halaman baru [Setup Fushi (Windows)](Setup-Fushi.md) (masih draf), muncul di menu Setup Mining > PC: cara instal, panduan awal di aplikasi, pasang kamus, kirim kartu ke Anki dengan note type Lapis, dan pasang ekstensi browser
       - Cara menambah sumber manga dan anime online di Fushi, lalu mencari judul dari dalam aplikasi
       - Cara membaca dialog visual novel lewat Fushi dan membuat kartu dari dialognya, lengkap dengan gambar bergerak dan suara karakter
       - Masalah umum Fushi: layar "Old data needs an upgrade first", hasil pencarian kosong, ekstensi browser belum terdeteksi, dan kartu tidak masuk ke Anki

*Panduan Gaya Penulisan*

- Untuk Penulis
       - Ada [panduan gaya penulisan](https://github.com/phi-li-a/philiaspace.my.id/blob/main/PANDUAN-GAYA.md) di repo: menyapa pembaca dengan "kamu", memakai "tidak" dan bukan "nggak", dan istilah yang diseragamkan seperti unduh, pasang, pengaturan, dan immersion
       - Semua halaman panduan akan disunting bertahap mengikuti panduan gaya ini supaya bahasanya seragam
- Pembaruan
       - Alamat halaman [Kartu Anime Satu Klik](kartu-anime-satu-klik.md) berubah dari `/Auto-Mining%20Anime/` menjadi `/kartu-anime-satu-klik/`, jadi tautan lama yang tersimpan perlu diganti

*Penyuntingan Bahasa Tahap 1*

- Pembaruan
       - Bahasa di [30 Hari Awal](rutinitas-awal.md), [Panduan Ringkas](panduan-ringkas-JP.md), [Belajar Kanji](kanji.md), dan [Perbaiki Font](font.md) dirapikan agar seragam dengan [Panduan Bahasa Jepang](panduan.md) dan lebih mudah dibaca
       - Langkah-langkah di [Perbaiki Font](font.md) sekarang bernomor, satu tindakan per langkah
- Perbaikan
       - [Panduan Ringkas](panduan-ringkas-JP.md): tombol Anki yang tertukar (Hard itu ++2++, Easy itu ++4++), dan semua langkah sekarang menyebut dek Kaishi yang sama
       - [Perbaiki Font](font.md): contoh kode styling kartu Anki yang sebelumnya tidak jalan kalau disalin, dan alamat folder Windows yang tampil dengan garis miring ganda
       - [Belajar Kanji](kanji.md): tautan 生ビール yang sebelumnya membuka kata lain
       - Pintasan keyboard di halaman panduan sekarang tampil dengan tanda "+" di antara tombol, misalnya Ctrl+Shift+A

*Sinkronisasi 30 Hari Awal*

- Pembaruan
       - [30 Hari Awal](rutinitas-awal.md) disamakan dengan versi terbaru UsagiSpoon di TheMoeWay: pengaturan Anki di Hari 4 dan Hari 8 sekarang memakai FSRS, learning steps `10m`, dan kartu baru muncul setelah ulasan
       - Hari 4 sekarang menawarkan pilihan dek kosakata yang sama dengan [Panduan Bahasa Jepang](panduan.md), dengan Kaishi V2 sebagai pilihan utama
       - Hari 4: ada cara menyalakan terjemahan otomatis subtitle YouTube, karena video Anki-nya hanya punya subtitle Inggris
       - Langkah "Learn ahead limit" dihapus karena sudah tidak ada di versi aslinya
       - Hari 1: tiga video kana bisa ditonton langsung di halaman
       - Setiap hari sekarang dipisah garis supaya batas antarhari lebih jelas
       - Bagian-bagian utama di halaman panduan lain juga dipisah garis dengan cara yang sama
- Perbaikan
       - Hianime yang sudah mati diganti Anikoto (subtitle Inggris yang bisa dimatikan) dan Sankanime (subtitle Indonesia yang menempel)
       - Tautan asbplayer di [30 Hari Awal](rutinitas-awal.md), [Anime MacOS](setup-anime-pc-lazy-guide.md), dan [Anime Android](setup-anime-android-lazy-guide.md) diganti ke alamat barunya
       - Daftar rekomendasi anime di Hari 2 yang sebelumnya berupa tabel berantakan sekarang jadi daftar biasa

*Penyuntingan Bahasa Tahap 2*

- Pembaruan
       - Bahasa di semua halaman LazyGuide dirapikan mengikuti panduan gaya: [Pengantar](setup.md), [Anki PC](setup-anki-pc-lazy-guide.md), [Yomitan PC](setup-yomitan-pc-lazy-guide.md), [Yomitan Android](setup-yomitan-android-lazy-guide.md), [ShareX](setup-ShareX-pc.md), Anime, LN & Buku, dan Manga untuk PC dan Android, serta [Memperbarui Note Type](pembaruan-note-type.md)
       - Judul bagian di halaman-halaman itu ikut diseragamkan, misalnya "Download dan Install" jadi "Unduh dan Pasang" dan "FAQs" jadi "Pertanyaan Umum", jadi tautan ke bagian lama yang tersimpan perlu diganti
       - Langkah untuk HP sekarang memakai "tekan", langkah untuk PC memakai "klik"
- Perbaikan
       - [Yomitan PC](setup-yomitan-pc-lazy-guide.md): judul halaman yang sebelumnya tidak tampil sebagai judul
       - [Anki PC](setup-anki-pc-lazy-guide.md): tombol Anki yang tertukar (Hard itu ++2++, Easy itu ++4++)
       - [Manga PC](setup-manga-pc-lazy-guide.md): perintah PowerShell untuk menghapus Python bawaan Windows yang diawali kata `input` sehingga gagal kalau disalin, dan sub-poin langkah OCR yang tampil sebagai langkah bernomor terpisah
       - [Anime MacOS](setup-anime-pc-lazy-guide.md): tombol untuk membuka `Load Subtitles` yang tampil rusak
       - Tautan sumber Yomitan Local Audio diarahkan ke repo barunya, dan alamat folder Anki di beberapa halaman tidak lagi menampilkan tanda bintang

*Penyuntingan Bahasa Tahap 3*

- Pembaruan
       - Bahasa di [Setup Manatan](Setup-Manatan.md), [Manga Lokal](Setup-Manatan-manga-lokal.md), [Anime Lokal](Setup-Manatan-anime-lokal.md), [Novel (EPUB)](Setup-Manatan-novels.md), [Kartu Anime Satu Klik](kartu-anime-satu-klik.md), dan [Yomitan & Anki PC](setup-yomitan-pc.md) dirapikan mengikuti panduan gaya; dengan ini semua halaman panduan sudah disunting
       - Judul bagian di halaman-halaman itu ikut diseragamkan (misalnya "FAQs" jadi "Pertanyaan Umum"), jadi tautan ke bagian lama yang tersimpan perlu diganti
       - [Yomitan & Anki PC](setup-yomitan-pc.md) sekarang punya baris tanggal unggah dan pembaruan seperti halaman lain
- Perbaikan
       - [Setup Manatan](Setup-Manatan.md): daftar di bagian Info, Tips, dan Pertanyaan Umum yang tampil berantakan, serta saran "pasang sumber anime" di bagian manga yang seharusnya "sumber manga"
       - [Yomitan & Anki PC](setup-yomitan-pc.md): tiga gambar langkah impor kamus yang kalau diklik membuka gambar lain
       - Nama kamus 三省堂国語辞典第八版, BCCWJ, dan YouTube di daftar kamus Manatan dan Yomitan & Anki PC
       - Label di beranda disesuaikan dengan menu: "Anime (Desktop)" untuk Kartu Anime Satu Klik, "Manatan (PC & HP)", dan Yomipv masuk daftar alat

**04-11-2026**

*Beranda*

- Landing Page & Desain
       - Beranda dibangun ulang sebagai landing page penuh tanpa sidebar dan daftar isi: hero gelap dengan contoh alur sentence mining (subtitle → Yomitan → Anki), tiga kartu fase pembelajaran, daftar alat gratis, blok ajakan Discord, kartu teori dan donasi
       - Footer khusus beranda (lockup 愛間 Philia Space, tautan GitHub, Discord, TikTok, Proyek komunitas, Riwayat perubahan, Donasi) menggantikan footer bawaan tema
       - Desain mengikuti brand guideline baru Philia Space: warna Langit `#00bbff`, netral Ink dan Malam, aksen Krim, radius 16 px, tombol pil
- Tampilan & Antarmuka
       - Font Plus Jakarta Sans dimuat dari `docs/fonts` dan dipakai untuk teks Latin di beranda serta tombol situs
       - Entri "Beranda" dihapus dari navigasi samping; kembali ke beranda lewat logo di header
- Perbaikan
       - Teks di atas warna biru Langit diganti ke Ink (`#111827`): kontras putih di atas `#00bbff` hanya 2.2:1 dan tidak lolos WCAG
       - Gaya kartu dan grid lama dipertahankan untuk halaman [Proyek Komunitas](proyek.md)
       - Daftar poin di [Panduan Bahasa Jepang](panduan.md) yang menyatu jadi satu baris diperbaiki; baris alur membaca yang tampil sebagai rumus mentah diganti teks biasa
       - Tautan mati gohoneko di Panduan (kuis kana, Tae Kim, Sakubi) diganti ke situs yang hidup
- Pembaruan Konten
       - [Panduan Bahasa Jepang](panduan.md) ditulis ulang dengan register lebih santai; istilah "imersi" diseragamkan jadi "immersion"
       - Bagian 3.1 sampai penutup dilokalisasi ulang mengikuti TheMoeWay versi terbaru (output sejak awal, pelafalan, tolok ukur kemajuan, penutup soal mining)
       - Disamakan dengan TheMoeWay: target belajar kana 3 minggu sampai sebulan, tiga level menyimak, dan catatan boleh menonton tanpa takarir sejak belajar kana
       - Video kana jadi tab (ENG) dengan tambahan Hiragana dan Katakana berbahasa Indonesia (IDN) dari Ryu Sensei; kuis kana ke DJT Guide dan Philia Shizen; Tadoku ke Level Start versi Inggris; kamus ke JIDict beserta cara pasang sebagai aplikasi di iOS dan Android
       - Penilaian kartu Anki jadi tabel centang/silang; alur harian jadi tabel; tangkapan layar halaman unduh Anki diperbarui (versi 26.09.3) dengan catatan AnkiMobile iOS berbayar
       - Tautan diperbarui: Kaishi (JP-EN), dek komunitas Discord, transkrip Cure Dolly ke kellenok.github.io
- Penambahan
       - Halaman baru [Proyek Komunitas](proyek.md): JIDict sebagai proyek utama (deskripsi, cara pasang, tautan repo dan versi web) serta alat buatan komunitas lainnya (Philia Bunrei, Tes Frekuensi Kosakata, Jimaku Bunseki, Shizen, Philia Kensaku, JobApp Mailer)
       - Entri navigasi "Proyek Komunitas" dan tautan dari beranda
       - Tautan TikTok @philiaspace.id di beranda dan halaman proyek

*Sinkronisasi LazyGuide*

- Pembaruan
       - [Setup Manga PC](setup-manga-pc-lazy-guide.md): MangaOCR diganti owocr dengan Screen AI (Google Lens lokal) sebagai engine bawaan, termasuk perintah shortcut di Info 1
       - [Setup Manga PC](setup-manga-pc-lazy-guide.md): Python untuk OCR dan Mokuro naik ke 3.13.9; panduan CUDA tidak lagi terkunci di versi 11.8
       - [Setup Anki PC](setup-anki-pc-lazy-guide.md): langkah FSRS disesuaikan dengan FSRS 6 (Optimize Current Preset tiap bulan, opsi FSRS Helper > Reschedule all cards); Desired Retention disamakan dengan screenshot (85%)
       - Tautan OCR di [Setup ShareX](setup-ShareX-pc.md) diarahkan ke bagian baru
- Penambahan
       - Opsi Firefox di [Setup Yomitan Android](setup-yomitan-android-lazy-guide.md), [LN Android](setup-LN-android-lazy-guide.md), dan [Manga Android](setup-manga-android-lazy-guide.md)
       - Info 4 di [Setup Anki PC](setup-anki-pc-lazy-guide.md): diagram troubleshooting interval FSRS
- Perbaikan
       - Semua tautan JIDict (Google Drive, Discord) diarahkan ke repo resmi [JIDict-yomitan](https://github.com/philiaspaceai/JIDict-yomitan); tautan JMDict Trilingual JP-EN-ID (beta) dihapus
       - `MainDefinition` JIDict di [Setup Yomitan PC](setup-yomitan-pc-lazy-guide.md) disesuaikan ke versi 1.0.3
       - Alamat folder MacOS yang memakai nama user `macbookair` diganti ke `~/Library/Application Support/Anki2` (Setup Anki PC, Panduan Ringkas, Local Audio di Setup Yomitan PC), ditambah cara membukanya lewat Finder > Go to Folder
       - Pembaca EPUB TTSU Reader (`reader.ttsu.app`) diganti ke [Yatsu Reader](https://app.yatsu.moe/), termasuk namanya di Setup LN PC & Android, beranda, dan config AnkiConnect di Setup Manga PC serta Yomitan & Anki PC
       - Tanggal entri April diperbaiki ke 2026

*Repo Baru*

- Perbaikan
       - Tombol GitHub di header dan tautan GitHub di footer beranda diarahkan ke repo baru [Philia-Space/philiaspace.my.id](https://github.com/Philia-Space/philiaspace.my.id)
       - Tombol "Edit this page" sekarang membuka branch `main` di repo baru (sebelumnya mengarah ke branch `master` yang tidak ada, jadi 404)
- Penambahan
       - Brand guideline Philia Space di folder `brand/` repo dan konvensi penamaan file lintas platform di README (khusus kontributor, tidak tampil di situs)

*Bahasa Antarmuka*

- Tampilan & Antarmuka
       - Antarmuka situs memakai bahasa Indonesia: "On this page" jadi "Di halaman ini", tombol navigasi bawah "Previous"/"Next" jadi "Sebelumnya"/"Selanjutnya", begitu juga kolom pencarian dan tombol ubah halaman
- Pembaruan Konten
       - Keterangan "Adaptasi TheMoeWay" di beranda dihapus karena panduan di situs ini diadaptasi dari beberapa sumber

*Menu di HP*

- Perbaikan
       - Sub-menu di menu samping HP tidak lagi bergeser dan menumpuk dengan menu sebelumnya, dan tombol kembali (←) di atasnya muncul lagi

*Deck Kaishi*

- Pembaruan
       - Deck Kaishi 1.5k Indonesia Simplified diganti ke Kaishi V2 di [Panduan Ringkas](panduan-ringkas-JP.md) dan [Panduan Bahasa Jepang](panduan.md)
- Penambahan
       - Pilihan deck sesuai tujuan di kedua halaman tersebut: Kaishi V2 untuk mulai immersion, Kaishi 1.5k versi RenRen, serta Multilingual Eggrolls JLPT 10k dan Ankidrone Essential V9 untuk JLPT

*Kartu Anime Satu Klik*

- Pembaruan
       - [Kartu Anime Satu Klik](kartu-anime-satu-klik.md): Autocards diganti Yomipv, yang bisa cari arti dan bikin kartu langsung di MPV dan bisa dipakai di Windows, Linux, dan macOS; di menu namanya sekarang "Anime Desktop" (sebelumnya "Anime Windows")
       - [Kartu Anime Satu Klik](kartu-anime-satu-klik.md): ada perintah siap copy-paste untuk PowerShell dan Terminal buat cek apakah semua prasyarat sudah terpenuhi
       - [Kartu Anime Satu Klik](kartu-anime-satu-klik.md): bagian FAQ baru berisi terjemahan dokumentasi Yomipv soal jendela kamus, warna subtitle sesuai status kartu, AniList, dan cara atur definisi yang masuk ke kartu
       - Tombol "sebelumnya/berikutnya" di bawah halaman dan teks lain bawaan situs sekarang berbahasa Indonesia
- Perbaikan
       - Tautan (?) ke halaman cara ekstrak file dihapus dari langkah ekstrak di Panduan Ringkas, Setup Anki PC, dan Setup Yomitan PC & Android

*Memperbarui Note Type*

- Penambahan
       - [Memperbarui Note Type](pembaruan-note-type.md): halaman baru untuk update semua note type yang dipakai di panduan (Lapis, Kiku, Senren, dan Mining-JP), lengkap dengan tabel note type mana dipakai di panduan mana
- Pembaruan
       - Halaman Memperbarui Format Lapis digabung ke halaman di atas; di menu Setup Lain namanya sekarang "Memperbarui Note Type"
       - Catatan bahwa Kiku sangat bergantung pada Anki desktop dan masih punya bug tampilan di iPhone/iPad, di halaman tersebut dan di [Setup Manatan](Setup-Manatan.md)

*Panduan Manatan*

- Pembaruan
       - [Setup Manatan](Setup-Manatan.md) disesuaikan dengan Manatan versi baru (tampilan aplikasi, bukan Web UI lagi), mengikuti dokumentasi resmi di manatan.com: download dari halaman resmi (termasuk App Store untuk iPhone/iPad), langkah setup awal, dan cara impor kamus
       - Note type bawaan Manatan sekarang Manatan-NoteType, bukan Kiku; Kiku dan Lapis tetap bisa dipakai dengan tabel field di bagian Kartu Flashcard
       - Bagian Masalah Umum diperbarui: Manatan tidak terbuka, popup kamus tidak muncul, kartu tidak masuk ke Anki, dan peringatan untuk backup dulu sebelum reset data
       - [Manga Lokal](Setup-Manatan-manga-lokal.md): file tunggal di folder utama, manga EPUB, format gambar yang didukung, dan saran memilih struktur folder
       - [Novel (EPUB)](Setup-Manatan-novels.md): tips membaca dan cara mengecek kalau popup kamus tidak muncul
       - Kamus JP-ID JPdict di [Setup Manatan](Setup-Manatan.md) diganti RH Dict (di Discord Philia Space)
- Penambahan
       - Bagian Kartu Flashcard di [Setup Manatan](Setup-Manatan.md): menyimpan kata ke Manatan SRS atau ke Anki lewat AnkiConnect
       - FAQ baru: apakah Manatan butuh browser, apakah OCR jalan offline, dan apakah sumber anime/manga sudah termasuk
- Perbaikan
       - Tautan Manga lokal dan Anime lokal di bagian Masalah Umum Setup Manatan yang sebelumnya rusak

---

### Oktober

**31-10-2026**

- Landing Page & Desain
       - Pembaruan beranda dokumentasi (`index.md`) bergaya Nextra docs: navigasi roadmap 3 fase (Fondasi, Tooling, Immersion), katalog setup perangkat (Desktop & Mobile), dan kanal komunitas
       - Penyesuaian proporsi visual: reduksi ukuran header 25% dan kartu hero landing page 50%
- Tampilan & Antarmuka
       - Pembaruan layout dokumentasi bergaya Nextra docs dengan header & sidebar terkunci (*isolated scrolling*)
       - Penyelarasan tema gelap (*slate mode*) dengan palet warna biru logo Philia Space (`#00bbff` dan `#38bdf8`)
       - Pembaruan logo situs di header dan icon tab browser (*favicon*) memakai logo resmi baru Philia Space
       - Perbaikan navigasi pagination footer (Previous & Next): lebar tombol simetris seimbang 50/50 dan judul panjang tidak terpotong (*no clipping*)
       - Pembaruan tombol donasi di header dengan ikon hati
       - Perbaikan styling komponen callout (*admonition*) agar rapi dan menyatu dengan alur teks
- Pembaruan Konten
       - Penyuntingan komprehensif naskah [Panduan Bahasa Jepang](panduan.md) agar lebih natural, sistematis, dan terstruktur
       - Pembaruan tautan panduan keyboard Jepang macOS di [Rutinitas Awal](rutinitas-awal.md) ke panduan resmi Apple Indonesia

---

### April

**13-04-2026**

- Umum
       - Pembaruan tautan Grinding Kana game
- Setup Utama
       - Penambahan Panduan [Setup Manatan](Setup-Manatan.md)
- Setup PC
       - Penambahan Panduan [Mining Windows](kartu-anime-satu-klik.md)
	   
---

## 2025

---

### September

**05-09-2025**

- Umum
       - Penambahan Tombol Repository Github Situs Philiaspace
       - Pembaruan format publikasi
       - Perbaikan typo dan kerapihan dokumentasi

---

### Agustus

**25-08-2025**

- Setup Utama
       - Pembaruan FAQ [Setup Yomitan PC](setup-yomitan-pc-lazy-guide.md)
       - Pembaruan FAQ [Setup Yomitan Android](setup-yomitan-android-lazy-guide.md)

**24-08-2025**

- Umum
       - Pembaruan susunan dokumentasi
- Setup Utama
       - Penambahan halaman [Setup Yomitan Android](setup-yomitan-android-lazy-guide.md)
       - Penambahan halaman [Setup ShareX](setup-ShareX-pc.md)
- Setup PC
       - Penambahan halaman [Setup Manga](setup-manga-pc-lazy-guide.md)
- Setup Android
       - Penambahan halaman [Setup Anime](setup-anime-android-lazy-guide.md)
       - Penambahan halaman [Setup LN & Buku](setup-LN-android-lazy-guide.md)
       - Penambahan halaman [Setup Manga](setup-manga-android-lazy-guide.md)

**10-08-2025**

- Umum
       - Perbaikan typo sana-sini dan merapikan formatting di berbagai bagian dokumentasi
- Panduan
       - Penambahan halaman [Panduan Bahasa Jepang](panduan.md)
       - Penambahan halaman [30 Hari Awal](rutinitas-awal.md)
       - Penambahan halaman [Perbaiki Font](font.md)
       - Penambahan halaman [Belajar Kanji](kanji.md)
       - Pembaruan halaman [Panduan Ringkas Bahasa Jepang](panduan-ringkas-JP.md)
- Setup
       - Penambahan halaman [Setup PC (Novel & Buku)](setup-LN-pc-lazy-guide.md)
       - Pembaruan halaman [Setup Anime](setup-anime-pc-lazy-guide.md)
       - Pembaruan halaman [Setup Anki](setup-anki-pc-lazy-guide.md)

**03-08-2025**

- Umum
       - Penambahan halaman [Panduan Ringkas Bahasa Jepang](panduan-ringkas-JP.md)
       - Penambahan ikon laman

**02-08-2025**

- Umum
	- Penambahan halaman beranda
- Pengaturan
	- Penambahan halaman [pengantar](setup.md)
	- Perbaikan dokumen

**01-08-2025**

- Umum
	- Pembaruan halaman [join discord](join.md)
- Pengaturan Utama
	- Penambahan tutorial [Anki PC (LazyGuide)](setup-anki-pc-lazy-guide.md)
	- Penambahan tutorial [Yomitan (LazyGuide)](setup-yomitan-pc-lazy-guide.md)
- Pengaturan PC
	- Penambahan tutorial [Mining Anime](setup.md)
- Lain-lain
	- Penambahan Riwayat Perubahan


---