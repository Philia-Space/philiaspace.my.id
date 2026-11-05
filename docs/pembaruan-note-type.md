---
hide:
  - footer
---
# Memperbarui Note Type
---

 Diunggah: 4 November 2026 – `Yaaacha`

---

Begini cara memperbarui note type (format kartu) Anki kamu, entah untuk memperbaiki bug atau sekadar mengikuti versi terbaru. Panduan di situs ini memakai beberapa note type:

| Note type | Dipakai di |
|---|---|
| [Lapis](https://github.com/donkuri/lapis) | Hampir semua panduan, mulai dari [Setup Anki PC](setup-anki-pc-lazy-guide.md) |
| [Kiku](https://github.com/youyoumu/kiku) | Opsional di [Manatan](Setup-Manatan.md) (bawaannya sekarang Manatan-NoteType, yang dipasang otomatis oleh Manatan), kompatibel dengan pengaturan Lapis. Butuh Anki desktop, kurang cocok kalau kamu lebih sering mengerjakan ulasan di HP |
| [Senren](https://github.com/BrenoAqua/Senren) | Bawaan Yomipv di [Kartu Anime Satu Klik](kartu-anime-satu-klik.md) |
| [Mining-JP](https://github.com/rudnam/JP-study#anki-mining-template) | [Setup Yomitan & Anki PC](setup-yomitan-pc.md) dan contoh di panduan anime |

Caranya mirip untuk semua note type: cadangkan kartu, unduh file `.apkg` terbaru, lalu impor ke Anki. Bedanya hanya di beberapa langkah kecil, jadi pilih tab sesuai note type yang kamu pakai.

!!!warning "Cadangkan dulu kartu-kartumu"
    Kamu **wajib** mencadangkan dek kamu dulu untuk jaga-jaga.

    1. Klik kanan dek kamu di Anki
    2. Pilih `Export`
    3. Centang opsi `Include scheduling information`, `Include Deck presets`, dan `Include Media`

---

## Opsi Import

Saat mengimpor file `.apkg`, Anki menampilkan jendela `Import options`. Untuk memperbarui note type, atur opsinya seperti ini, lalu klik `Import`:

- `Import any learning progress`: mati
- `Import any deck presets`: mati
- `Merge note types`: **nyala**
- `Update notes`: `Always`
- `Update note types`: `Always`

![Opsi impor untuk memperbarui note type](img/lapis-import-update.png){height=300 width=600}

`Merge note types` harus menyala. Kalau tidak, Anki akan membuat note type baru (misalnya `Lapis-xxxx`), sedangkan kartu lamamu tetap memakai versi lama.

---

## Cara Memperbarui

=== "Lapis"

    Butuh Anki 23.10 atau lebih baru.

    1. Salin dulu perubahan di bagian `Styling` Lapis kalau kamu pernah mengubah variabelnya (misalnya ukuran font atau warna). Pembaruan akan mengembalikan semuanya ke bawaan
    2. Unduh versi terbaru [Lapis](https://github.com/donkuri/lapis/releases/latest)
        - Gulir ke bawah ke bagian `Assets`, lalu cari file `Lapis.apkg`

        ![lapis apkg](img/lapis-apkg.png){height=150 width=300}

    3. Buka file `Lapis.apkg` di Anki, atur [opsi impor](#opsi-import), lalu klik `Import`
    4. Hapus dek `Lapis` dari layar utama (kalau sebelumnya kamu sudah mengganti nama dek lama jadi `Mining Deck`)
    5. Tempel lagi perubahan `Styling` dari langkah 1 kalau ada
    6. Selesai!

=== "Kiku"

    Butuh **Anki 25.09** atau lebih baru, dan add-on [Kiku Note Manager](https://ankiweb.net/shared/info/408592650).

    !!!warning "Kiku sangat bergantung pada Anki desktop"
        - Kiku hanya bisa dipasang dan diperbarui lewat Anki di PC, karena add-on Kiku Note Manager hanya ada di versi desktop
        - Fitur Kanji Web di HP butuh cache yang dibuat di PC. Cache ini tidak diperbarui otomatis, jadi setelah menambah kartu baru kamu perlu membuatnya ulang di PC, lalu sync
        - **AnkiDroid**: sudah diuji oleh pembuatnya, tapi tetap terkena keterbatasan di atas
        - **AnkiMobile (iOS)**: masih ada [beberapa bug tampilan](https://github.com/youyoumu/kiku/issues/12), misalnya popup kanji tidak bisa ditutup dengan menekan di luar popup, serta posisi tombol audio dan gambar yang meleset

        Kalau kamu lebih sering mengerjakan ulasan di HP, terutama di iPhone atau iPad, [Lapis](https://github.com/donkuri/lapis) lebih aman dipakai.

    1. Unduh file `Kiku_v*.apkg` terbaru dari [halaman rilis Kiku](https://github.com/youyoumu/kiku/releases/latest)
    2. Hapus file Kiku yang lama dulu: `Tools` > `Kiku Note Manager` > `Delete Kiku files`
        - Langkah ini wajib, karena Anki tidak mau menimpa file yang sudah ada. Kalau dilewati, kartumu tetap memakai file versi lama
        - Pengaturanmu (`_kiku_config.json`, `_kiku_plugin.js`, `_kiku_plugin.css`) tidak ikut terhapus
    3. Buka file `.apkg` tadi di Anki, atur [opsi impor](#opsi-import), lalu klik `Import`
    4. Buka halaman pengaturan Kiku, lalu klik `Save` supaya template kartu disesuaikan dengan pengaturanmu
    5. Selesai!

    Kalau fitur Kanji Web tidak muncul di HP, buat ulang cache-nya lewat `Tools` > `Kiku Note Manager` > `Generate notes cache`.

    Sumber: [Updating Kiku](https://kiku.youyoumu.my.id/updating.html)

=== "Senren"

    1. Unduh file `Senren.v*.apkg` terbaru dari [halaman rilis Senren](https://github.com/BrenoAqua/Senren/releases/latest)
    2. Buka file itu di Anki (`File` > `Import`, atau ++ctrl+shift+i++), atur [opsi impor](#opsi-import), lalu klik `Import`
    3. Selesai!

    ??? info "Memperbarui tanpa mengunduh .apkg <small>(klik di sini)</small>"

        1. Buka `Browse` di Anki
        2. Pilih note type `Senren`, lalu klik `Cards`
        3. Ganti seluruh isi `Front Template`, `Back Template`, dan `Styling` dengan isi file berikut:
            - [front.html](https://github.com/BrenoAqua/Senren/raw/refs/heads/main/Template/front.html)
            - [back.html](https://github.com/BrenoAqua/Senren/raw/refs/heads/main/Template/back.html)
            - [styling.css](https://github.com/BrenoAqua/Senren/raw/refs/heads/main/Template/styling.css)
        4. Simpan

    Sumber: [Senren Setup](https://brenoaqua.github.io/Senren/setup_overview/)

=== "Mining-JP"

    Mining-JP tidak punya rilis bernomor versi. Filenya terakhir diperbarui Juni 2024, jadi kalau kamu memasangnya setelah itu, kemungkinan besar kamu sudah memakai versi terbaru.

    1. Salin dulu perubahanmu kalau kamu pernah mengubah template atau `Styling`-nya (misalnya supaya mengikuti tema sistem)
    2. Unduh [Mining_temp.apkg](https://github.com/rudnam/JP-study/raw/main/Mining_temp.apkg)
    3. Buka file itu di Anki, atur [opsi impor](#opsi-import), lalu klik `Import`
    4. Tempel lagi perubahan dari langkah 1 kalau ada
    5. Selesai!

    Sumber: [JP-study](https://github.com/rudnam/JP-study#anki-mining-template)

---
