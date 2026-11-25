---
description: "Cara memindahkan kartu Anki dari note type lain (Lapis, Mining-JP, Anime Cards, dan lainnya) ke jp-mining-note tanpa kehilangan jadwal ulasan."
hide:
  - footer
---
# Pindah ke jp-mining-note

!!! info "Diadaptasi dari jp-mining-note"
    Halaman ini diadaptasi dari [Transfer Existing Notes](https://aquafina-water-bottle.github.io/jp-mining-note/importing/) di dokumentasi jp-mining-note, ditulis oleh **Aquafina-water-bottle**.

    Tabel pemetaan untuk Lapis dan Mining-JP ditambahkan oleh Philia Space. Tabel Anime Cards dan langkah merapikan kartu berasal dari versi aslinya.

    Versi aslinya berlisensi [MIT](https://github.com/Aquafina-water-bottle/jp-mining-note/blob/master/LICENSE), halaman ini berlisensi GPL-3.0 (rinciannya di [lisensi Philia Space](https://github.com/Philia-Space/philiaspace.my.id/blob/main/LICENSE.docs.md)). Kalau kamu nyaman baca bahasa Inggris, baca [versi aslinya](https://aquafina-water-bottle.github.io/jp-mining-note/importing/).

---

[jp-mining-note](https://aquafina-water-bottle.github.io/jp-mining-note/) adalah note type mining yang sangat kaya fitur: pitch accent berwarna, tooltip kata lain di kartu, banyak jenis kartu, dan bisa diubah tampilannya. Halaman ini menjelaskan cara memindahkan kartu yang sudah kamu punya dari note type lain ke jp-mining-note. Jadwal ulasan kartu lamamu tetap terbawa.

!!! warning "Dokumentasi aslinya ditulis tahun 2023"
    - Dokumentasi jp-mining-note masih menyebut **Yomichan**. Sekarang penggantinya adalah Yomitan, dan pengaturannya hampir sama.
    - Pengembangan jp-mining-note dilanjutkan di [fork arbyste](https://arbyste.github.io/jp-mining-note-prerelease/). Cek versi yang kamu pasang, karena nama field atau perintah bisa berubah di versi baru.
    - Philia Space sendiri memakai [Lapis](https://github.com/donkuri/lapis). Pilih jp-mining-note kalau kamu memang butuh fiturnya dan siap mengatur lebih banyak hal.

Beberapa hal yang perlu kamu tahu dulu:

- Tidak semua isi kartu bisa pindah 100%. Yang paling sering hilang adalah daftar frekuensi, karena jp-mining-note memakai format sendiri.
- Kalau kamu hanya ingin memperbarui jp-mining-note versi lama ke versi baru, **jangan** pakai halaman ini. Ikuti [Updating](https://aquafina-water-bottle.github.io/jp-mining-note/updating/) di dokumentasinya.

---

## Sebelum Mulai

1. Pasang jp-mining-note dan add-on yang dibutuhkannya lewat [Setup: Anki](https://aquafina-water-bottle.github.io/jp-mining-note/setupanki/). Pastikan [AnkiConnect](https://ankiweb.net/shared/info/2055492159) dan [AJT Japanese](https://ankiweb.net/shared/info/1344485230) sudah terpasang.
2. Cadangkan koleksi Anki kamu.

!!! warning "Cadangkan dulu kartu-kartumu"
    Kamu **wajib** mencadangkan dek kamu dulu untuk jaga-jaga.

    1. Klik kanan dek kamu di Anki
    2. Pilih `Export`
    3. Centang opsi `Include scheduling information`, `Include Deck presets`, dan `Include Media`

    Mengganti note type seharusnya tidak mengubah berkas media (gambar dan audio), tapi menyertakan media di cadangan tetap lebih aman kalau ruang penyimpananmu cukup.

---

## Langkah 1: Ganti Note Type

1. Di layar utama Anki, klik `Browse`.
2. Pilih semua kartu yang mau dipindah. Tekan ++ctrl+a++ untuk memilih semua kartu yang tampil.
3. Klik kanan kartu yang dipilih, lalu pilih `Notes` > `Change Note Type...`
4. Di bagian atas jendela, pilih `JP Mining Note` sebagai note type tujuan.
5. Atur pasangan field sesuai [Langkah 2](#langkah-2-petakan-field), lalu klik `Save`.

Mengganti note type lewat cara ini tetap menyimpan jadwal ulasan kartu.

---

## Langkah 2: Petakan Field

Di jendela `Change Note Type`, tiap field jp-mining-note (kiri) diisi dari salah satu field note type lamamu (kanan). Aturan umumnya:

- Isi `Key` **dan** `Word` dari field kata yang sama. Kebanyakan note type hanya punya satu field kata, dan isi kedua field ini harus sama persis.
- Kosongkan `AJTWordPitch` dan `SentenceReading`. Keduanya bisa dibuat ulang sekaligus oleh AJT Japanese di [Langkah 3](#langkah-3-rapikan-kartu).
- Gambar pitch accent masuk ke `PAGraphs`. Posisi pitch accent (angka) masuk ke `PAPositions`. Warna pitch accent di kartu lama **hanya** muncul kalau `PAPositions` terisi dengan format jp-mining-note.
- Nilai frekuensi untuk mengurutkan kartu masuk ke `FrequencySort`.
- Nama media atau sumber kalimat masuk ke `AdditionalNotes`.
- `WordReading` paling bagus berisi furigana polos, misalnya `成[な]り 立[た]つ`. Kalau note type lamamu hanya menyimpan kana (`なりたつ`) atau furigana HTML, tetap petakan saja, lalu rapikan di [Langkah 3](#langkah-3-rapikan-kartu).
- **Jangan** isi `FrequenciesStylized`, walaupun kartu lamamu punya field daftar frekuensi. Field ini memakai format sendiri, dan isi dari `{frequencies}` Yomitan akan tampil berantakan.
- Field lain yang tidak punya pasangan dibiarkan `(Nothing)`.

Pilih tab sesuai note type lamamu. Tab Lapis dan Mining-JP disusun oleh Philia Space dari daftar field kedua note type itu. Coba dulu di beberapa kartu dan cek hasilnya sebelum memindahkan semuanya.

=== "Lapis"

    | Field jp-mining-note | Diisi dari field Lapis |
    |---|---|
    | `Key` | `Expression` |
    | `Word` | `Expression` |
    | `WordReading` | `ExpressionFurigana` |
    | `PrimaryDefinition` | `MainDefinition` |
    | `PrimaryDefinitionPicture` | `DefinitionPicture` |
    | `Sentence` | `Sentence` |
    | `HintNotHidden` | `Hint` |
    | `IsSentenceCard` | `IsSentenceCard` |
    | `IsClickCard` | `IsClickCard` |
    | `Picture` | `Picture` |
    | `WordAudio` | `ExpressionAudio` |
    | `SentenceAudio` | `SentenceAudio` |
    | `FrequencySort` | `FreqSort` |
    | `SecondaryDefinition` | `Glossary` |
    | `AdditionalNotes` | `MiscInfo` |
    | Field lain | `(Nothing)` |

    - Kalau kamu sering menyorot arti di popup Yomitan (field `SelectionText` terisi), pilih `SelectionText` untuk `PrimaryDefinition`.
    - `PitchPosition`, `PitchCategories`, dan `Frequency` dari Lapis tidak dipetakan, karena formatnya berbeda dengan jp-mining-note. Pitch accent dibuat ulang lewat AJT Japanese di Langkah 3.
    - Lapis tidak punya padanan untuk `IsWordAndSentenceCard` dan `IsAudioCard`. Kalau kamu memakainya, atur ulang jenis kartunya lewat [Card Types](https://aquafina-water-bottle.github.io/jp-mining-note/cardtypes/) jp-mining-note.
    - `ExpressionFurigana` Lapis sudah berupa furigana polos, jadi bagian merapikan `WordReading` di Langkah 3 bisa dilewati.

=== "Mining-JP"

    | Field jp-mining-note | Diisi dari field Mining-JP |
    |---|---|
    | `Key` | `Expression` |
    | `Word` | `Expression` |
    | `WordReading` | `ExpressionFurigana` |
    | `PrimaryDefinition` | `MainDefinition` |
    | `Sentence` | `Sentence` |
    | `HintNotHidden` | `Hint` |
    | `IsSentenceCard` | `IsSentenceCard` |
    | `Picture` | `Image` |
    | `WordAudio` | `ExpressionAudio` |
    | `SentenceAudio` | `SentenceAudio` |
    | `FrequencySort` | `FreqSort` |
    | `SecondaryDefinition` | `FullDefinition` |
    | `AdditionalNotes` | `MiscInfo` |
    | Field lain | `(Nothing)` |

    - `PitchPosition` dan `Frequency` tidak dipetakan karena formatnya berbeda. Pitch accent dibuat ulang lewat AJT Japanese di Langkah 3.
    - Kalau `Translation` atau `ExtraField` di kartu lamamu berisi sesuatu, petakan salah satunya ke `Comment` supaya isinya tidak hilang.
    - `ExpressionFurigana` Mining-JP sudah berupa furigana polos, jadi bagian merapikan `WordReading` di Langkah 3 bisa dilewati.

=== "Anime Cards"

    Contoh dari dokumentasi jp-mining-note untuk [Anime Cards](https://animecards.site/ankicards/).

    | Field jp-mining-note | Diisi dari field Anime Cards |
    |---|---|
    | `Key` | `front` |
    | `Word` | `front` |
    | `WordReading` | `Reading` |
    | `PrimaryDefinition` | `Glossary` |
    | `Sentence` | `Sentence` |
    | `HintNotHidden` | `Hint` |
    | `Picture` | `Picture` |
    | `WordAudio` | `Audio` |
    | `SentenceAudio` | `SentenceAudio` |
    | `PAGraphs` | `Graph` |
    | Field lain | `(Nothing)` |

=== "Note type lain"

    Belum ada tabel khusus untuk note type lain, misalnya Kiku, Senren, atau [note type lain di daftar ini](note-type.md). Pakai aturan umum di atas, lalu cocokkan field yang isinya sama:

    | Isi field | Field jp-mining-note |
    |---|---|
    | Kata | `Key` dan `Word` |
    | Bacaan atau furigana kata | `WordReading` |
    | Arti utama (ringkas) | `PrimaryDefinition` |
    | Arti lengkap atau kamus kedua | `SecondaryDefinition` |
    | Kalimat | `Sentence` |
    | Gambar | `Picture` |
    | Audio kata | `WordAudio` |
    | Audio kalimat | `SentenceAudio` |
    | Gambar grafik pitch accent | `PAGraphs` |
    | Angka frekuensi untuk mengurutkan | `FrequencySort` |
    | Nama media atau catatan | `AdditionalNotes` |

    Senren menyimpan beberapa adegan dalam satu kartu. Setelah pindah, semua kalimat dan gambarnya akan tampil berurutan di satu field, bukan lagi sebagai adegan yang bisa dipilih.

---

## Langkah 3: Rapikan Kartu

Kerjakan bagian di bawah ini berurutan. Bagian yang memakai Python butuh Anki dalam keadaan terbuka dan AnkiConnect terpasang.

### Format kalimat (`Sentence`)

jp-mining-note menandai kata yang dicari dengan tag `<b>`. Cek dulu isi HTML field `Sentence` di salah satu kartu: di editor Anki, klik field-nya lalu tekan ++ctrl+shift+x++.

- Kata sudah dibungkus `<b>...</b>`: sudah benar, lewati bagian ini. Kartu dari Lapis, Mining-JP, dan pengaturan Yomitan di situs ini sudah seperti ini.
- Tidak ada penanda sama sekali: lewati juga. jp-mining-note bisa [menyorot kata secara otomatis](https://aquafina-water-bottle.github.io/jp-mining-note/ui/#automatic-word-highlighting).
- Kata ditandai dengan cara lain, misalnya `<span style="color: ...">`: ubah ke `<b>` dengan langkah di bawah.

??? info "Mengubah penanda kata ke `<b>` <small>(klik di sini)</small>"

    1. Buat cadangan sekali lagi.
    2. Di `Browse`, pilih satu kartu lama, klik kanan, lalu pilih `Notes` > `Find and Replace...`
    3. Isi seperti ini:
        - `Find`: `<span style="color: #ffc2c7">(?P<t>.*?)</span>` (hampir pasti perlu kamu sesuaikan dengan format kartumu)
        - `Replace With`: `<b>$t</b>`
        - `In`: `Sentence`
        - `Selected notes only`: mati
        - `Ignore case`: mati
        - `Treat input as a regular expression`: nyala
    4. Klik `OK`, lalu buka kartunya. Kalau kata yang dicari sekarang tersorot kuning (biru di mode terang), berarti berhasil.
    5. Kalau gagal, sesuaikan isi `Find`. Panduan regex Anki ada di [dokumentasi Anki](https://docs.ankiweb.net/searching.html#regular-expressions).

### Buat ulang pitch accent dan furigana kalimat

Bagian ini opsional, tapi **sangat disarankan**. Kalau `PAPositions` kosong, pitch accent kemungkinan besar tidak tampil di kartu hasil pindahan. Butuh add-on AJT Japanese yang sudah [diatur untuk jp-mining-note](https://aquafina-water-bottle.github.io/jp-mining-note/setupanki/#ajt-japanese).

1. Di layar utama Anki, klik `Browse`.
2. Ketik `"note:JP Mining Note"` di kotak pencarian (tanda kutipnya ikut diketik), lalu tekan ++ctrl+a++.
3. Klik `Edit` di kiri atas, lalu pilih `AJT: Bulk-generate`.

### Isi field `PASilence`

Field ini perlu diisi supaya kartu pitch accent bekerja dengan benar ([penjelasannya](https://aquafina-water-bottle.github.io/jp-mining-note/faq/#what-is-the-point-of-the-pasilence-field)).

1. Di `Browse`, klik kanan salah satu kartu, lalu pilih `Notes` > `Find and Replace...`
2. Isi seperti ini:
    - `Find`: `.*`
    - `Replace With`: `[sound:_silence.wav]`
    - `In`: `PASilence` (**jangan sampai salah pilih field**)
    - `Selected notes only`: mati
    - `Ignore case`: mati
    - `Treat input as a regular expression`: nyala
3. Klik `OK`.

### Format bacaan kata (`WordReading`)

Lihat isi `WordReading` di salah satu kartu, lalu cocokkan dengan tiga kemungkinan ini:

| Isi `WordReading` | Contoh | Yang perlu dilakukan |
|---|---|---|
| Furigana polos (`{furigana-plain}`) | `成[な]り 立[た]つ` | Sudah benar, lewati |
| Furigana HTML (`{furigana}`) | <ruby>成<rt>な</rt></ruby>り<ruby>立<rt>た</rt></ruby>つ | Ubah dengan `Find and Replace` |
| Kana saja (`{reading}`) | `なりたつ` | Ubah dengan skrip Python |

??? info "Mengubah furigana HTML ke furigana polos <small>(klik di sini)</small>"

    1. Di `Browse`, klik kanan salah satu kartu, lalu pilih `Notes` > `Find and Replace...`
    2. Isi seperti ini:
        - `Find`: `<ruby>(<rb>)?(?P<kanji>.*?)(</rb>)?<rt>(?P<furigana>.*?)</rt></ruby>`
        - `Replace With`: ` $kanji[$furigana]` (spasi di depannya ikut diketik)
        - `In`: `WordReading`
        - `Selected notes only`: mati
        - `Ignore case`: mati
        - `Treat input as a regular expression`: nyala
    3. Klik `OK`.

??? info "Mengubah bacaan kana saja <small>(klik di sini)</small>"

    Hasilnya tidak sempurna, tapi cukup layak: kata dan bacaannya digabung jadi `成り立つ[なりたつ]`. Buat cadangan dulu.

    1. Pasang [Python](https://www.python.org/downloads/). Di Windows, ikuti tiga langkah pertama di [Running the script](https://aquafina-water-bottle.github.io/jp-mining-note/updating/#running-the-script).
    2. Unduh kode jp-mining-note dari [GitHub](https://github.com/Aquafina-water-bottle/jp-mining-note) (`Code` > `Download ZIP`), lalu ekstrak.
    3. Buka terminal di folder `jp-mining-note/tools`.
    4. Jalankan perintah ini. Perintah ini mengubah **semua** kartu jp-mining-note:

        === "Windows"

            ```
            python batch.py -f "quick_fix_convert_kana_only_reading_all_notes"
            ```

        === "MacOS dan Linux"

            ```
            python3 batch.py -f "quick_fix_convert_kana_only_reading_all_notes"
            ```

    Kalau hanya sebagian kartu yang bacaannya kana saja, beri tag `kanaonlyreading` ke kartu-kartu itu, lalu jalankan perintah ini sebagai gantinya:

    === "Windows"

        ```
        python batch.py -f "quick_fix_convert_kana_only_reading_with_tag"
        ```

    === "MacOS dan Linux"

        ```
        python3 batch.py -f "quick_fix_convert_kana_only_reading_with_tag"
        ```

### Isi `WordReadingHiragana` (opsional)

Field ini menyalakan [penanda kata](https://aquafina-water-bottle.github.io/jp-mining-note/ui/#word-indicators) di kartu lama. Butuh jp-mining-note versi 0.11.0.0 atau lebih baru, dan **baru boleh dijalankan setelah `WordReading` berisi furigana polos**.

Dari folder `jp-mining-note/tools`, jalankan:

=== "Windows"

    ```
    python batch.py -f "fill_word_reading_hiragana_field"
    ```

=== "MacOS dan Linux"

    ```
    python3 batch.py -f "fill_word_reading_hiragana_field"
    ```

### Isi `FrequencySort` (opsional)

Kalau kartu lamamu belum punya nilai frekuensi (kartu dari Lapis dan Mining-JP biasanya sudah punya lewat `FreqSort`), kamu bisa mengisinya belakangan dengan skrip dari MarvNC. Ikuti [Backfilling old cards](https://github.com/MarvNC/JP-Resources#backfilling-old-cards), lalu jalankan dengan pengaturan untuk jp-mining-note:

```
python backfill.py "Word" --freq-field "FrequencySort" --query "FrequencySort: \"note:JP Mining Note\""
```

---

## Yang Tidak Ikut Pindah

- **Daftar frekuensi.** Kartu lama tidak akan menampilkan daftar frekuensi seperti kartu baru. Belum ada alat untuk mengubah format `{frequencies}` ke format jp-mining-note.
- **Warna pitch accent tanpa `PAPositions`.** jp-mining-note tidak bisa membaca posisi pitch accent dari gambar grafik. Kalau `AJT: Bulk-generate` tidak mengisi pitch accent untuk sebagian kartu, kamu perlu mengisinya sendiri per kartu. Detailnya ada di [Colored Pitch Accent](https://aquafina-water-bottle.github.io/jp-mining-note/autopa/#colored-pitch-accent).
- **Fitur khusus note type lama**, misalnya adegan Senren atau field grouping Kiku.

Masih bingung? Cek [FAQ jp-mining-note](https://aquafina-water-bottle.github.io/jp-mining-note/faq/) atau tanya di [Discord Philia Space](join.md).
