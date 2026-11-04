---
hide:
  - footer
---
# Memperbarui Note Type
---

 Diunggah: 4 November 2026 – `Yaaacha`

---

Begini cara memperbarui note type (format kartu) Anki kamu, entah buat perbaiki bug atau sekadar update ke versi terbaru. Panduan di situs ini memakai beberapa note type:

| Note type | Dipakai di |
|---|---|
| [Lapis](https://github.com/donkuri/lapis) | Hampir semua panduan, mulai dari [Setup Anki PC](setup-anki-pc-lazy-guide.md) |
| [Kiku](https://github.com/youyoumu/kiku) | Bawaan [Manatan](Setup-Manatan.md), kompatibel dengan pengaturan Lapis. Butuh Anki desktop, kurang cocok kalau sering review di HP |
| [Senren](https://github.com/BrenoAqua/Senren) | Bawaan Yomipv di [Kartu Anime Satu Klik](Auto-Mining%20Anime.md) |
| [Mining-JP](https://github.com/rudnam/JP-study#anki-mining-template) | [Setup Yomitan & Anki PC](setup-yomitan-pc.md) dan contoh di panduan anime |

Caranya mirip untuk semuanya: backup, download file `.apkg` terbaru, lalu import ke Anki. Yang beda hanya beberapa langkah kecil, jadi pilih tab sesuai note type yang kamu pakai.

!!!warning "Pastikan backup dulu kartu-kartumu"
    Kamu **wajib** `backup` deck-mu dulu buat jaga-jaga

    1. Di Anki, klik kanan pada `deck` kamu
    2. Pilih `Export`
    3. Pastikan opsi-opsi ini dicentang: `Include scheduling information`, `Include Deck presets`, `Include Media`

---

## Opsi Import

Saat import file `.apkg`, Anki akan menampilkan jendela **Import options**. Untuk update, atur seperti ini lalu klik `Import`:

- `Import any learning progress`: mati
- `Import any deck presets`: mati
- `Merge note types`: **nyala**
- `Update notes`: **Always**
- `Update note types`: **Always**

![Opsi import untuk update note type](img/lapis-import-update.png){height=300 width=600}

`Merge note types` harus nyala. Kalau tidak, Anki akan membuat note type baru (misalnya `Lapis-xxxx`) dan kartu lamamu tetap memakai versi lama.

---

## Cara Update

=== "Lapis"

    Butuh Anki 23.10 atau lebih baru.

    1. Kalau kamu pernah mengubah variabel di bagian `Styling` Lapis (misalnya ukuran font atau warna), salin dulu perubahannya. Update akan mengembalikan semuanya ke bawaan
    2. Download versi terbaru [Lapis](https://github.com/donkuri/lapis/releases/latest)
        - Scroll ke bawah ke bagian *Assets*, lalu cari file `Lapis.apkg`

        ![lapis apkg](img/lapis-apkg.png){height=150 width=300}

    3. Buka file `Lapis.apkg` di Anki, atur [opsi import](#opsi-import), lalu klik `Import`
    4. Hapus deck `Lapis` dari layar utama (kalau sebelumnya kamu sudah ganti nama deck lama jadi `Mining Deck`)
    5. Tempel lagi perubahan `Styling` dari langkah 1 kalau ada
    6. Beres deh!

=== "Kiku"

    Butuh **Anki 25.09** atau lebih baru, dan add-on [Kiku Note Manager](https://ankiweb.net/shared/info/408592650).

    !!!warning "Kiku sangat bergantung pada Anki desktop"
        - Pasang dan update Kiku harus lewat Anki di PC, karena add-on Kiku Note Manager hanya ada di desktop
        - Fitur Kanji Web di HP butuh cache yang dibuat dari PC. Cache ini tidak ter-update sendiri, jadi setelah menambah kartu baru kamu perlu buat ulang di PC lalu sync
        - **AnkiDroid**: sudah diuji oleh pembuatnya, tapi tetap ikut keterbatasan di atas
        - **AnkiMobile (iOS)**: masih ada [beberapa bug tampilan](https://github.com/youyoumu/kiku/issues/12), misalnya popup kanji tidak bisa ditutup dengan tap di luar popup, dan posisi tombol audio serta gambar meleset

        Kalau kamu lebih sering review di HP, terutama iPhone/iPad, [Lapis](https://github.com/donkuri/lapis) lebih aman dipakai.

    1. Download file `Kiku_v*.apkg` terbaru dari [halaman rilis Kiku](https://github.com/youyoumu/kiku/releases/latest)
    2. Hapus file Kiku yang lama dulu: `Tools` > `Kiku Note Manager` > `Delete Kiku files`
        - Langkah ini wajib, karena Anki tidak mau menimpa file yang sudah ada. Kalau dilewati, kartumu tetap memakai file versi lama
        - Pengaturanmu (`_kiku_config.json`, `_kiku_plugin.js`, `_kiku_plugin.css`) tidak ikut terhapus
    3. Buka file `.apkg` tadi di Anki, atur [opsi import](#opsi-import), lalu klik `Import`
    4. Buka halaman pengaturan Kiku lalu klik `Save`. Ini menyamakan template kartu dengan pengaturanmu
    5. Beres deh!

    Kalau fitur Kanji Web tidak muncul di HP, buat ulang cache-nya lewat `Tools` > `Kiku Note Manager` > `Generate notes cache`.

    Sumber: [Updating Kiku](https://kiku.youyoumu.my.id/updating.html)

=== "Senren"

    1. Download file `Senren.v*.apkg` terbaru dari [halaman rilis Senren](https://github.com/BrenoAqua/Senren/releases/latest)
    2. Buka file itu di Anki (`File` > `Import`, atau ++ctrl+shift+i++), atur [opsi import](#opsi-import), lalu klik `Import`
    3. Beres deh!

    ??? info "Update tanpa download .apkg <small>(klik untuk buka)</small>"

        1. Buka `Browse` di Anki
        2. Pilih note type `Senren`, lalu klik `Cards`
        3. Ganti seluruh isi `Front Template`, `Back Template`, dan `Styling` dengan isi file ini:
            - [front.html](https://github.com/BrenoAqua/Senren/raw/refs/heads/main/Template/front.html)
            - [back.html](https://github.com/BrenoAqua/Senren/raw/refs/heads/main/Template/back.html)
            - [styling.css](https://github.com/BrenoAqua/Senren/raw/refs/heads/main/Template/styling.css)
        4. Simpan

    Sumber: [Senren Setup](https://brenoaqua.github.io/Senren/setup_overview/)

=== "Mining-JP"

    Mining-JP tidak punya rilis bernomor versi. File-nya terakhir diperbarui Juni 2024, jadi kalau kamu memasangnya setelah itu, kemungkinan besar sudah versi terbaru.

    1. Kalau kamu pernah mengubah template atau `Styling`-nya (misalnya mengikuti tema sistem), salin dulu perubahannya
    2. Download [Mining_temp.apkg](https://github.com/rudnam/JP-study/raw/main/Mining_temp.apkg)
    3. Buka file itu di Anki, atur [opsi import](#opsi-import), lalu klik `Import`
    4. Tempel lagi perubahan dari langkah 1 kalau ada
    5. Beres deh!

    Sumber: [JP-study](https://github.com/rudnam/JP-study#anki-mining-template)

---
