---
hide:
  - footer
---
# Isi Field Note Type di Manatan
---

 Diunggah: 11 November 2026 – `Yaaacha`

---

Manatan tidak punya pengaturan siap pakai untuk note type selain Manatan-NoteType. Kalau kamu memakai note type lain, field-nya harus kamu isi sendiri. Halaman ini berisi isian untuk note type yang dipakai di panduan situs ini.

Kalau kamu memakai **Manatan-NoteType**, kamu tidak perlu mengubah apa pun. Note type itu dipasang dan diatur otomatis oleh Manatan.

---

## Sebelum mulai

1. Pasang dulu note type-nya di Anki. Caranya ada di [Memperbarui Note Type](pembaruan-note-type.md).
2. Hubungkan Manatan ke Anki seperti di [Setup Manatan](Setup-Manatan.md#kartu-flashcard).
3. Buka `More` > ikon roda gigi > `Settings` > `Language learning` > `Flashcards`, lalu pilih note type-nya di `Card Type`.
4. Isi tiap field di bagian `Field mapping` sesuai tabel di bawah.
5. Atur bagian `Duplicates` di paling bawah halaman sesuai tabel.
6. Tambang satu kata, lalu cek kartunya di Anki sebelum menambang banyak kata.

Cara membaca tabel:

- **Isi** adalah pilihan di kolom `Card content`. Kalau tertulis `Custom Template`, pilih `Custom Template` lalu salin teks di bawahnya ke kotak `Custom Template`.
- **Kosong** berarti pilih `None`.
- **Update Mode** hanya berpengaruh kalau kata yang sama ditambang lagi dan `Duplicate Action` diatur ke `Overwrite`. Arti tiap pilihannya ada di [Setup Manatan](Setup-Manatan.md#isi-field-sesuai-note-type).
- `Single Glossary` perlu dipilih kamusnya lewat panah di samping kolom. Pakai kamus yang isinya ringkas, misalnya JMdict atau JIDict.

!!! tip "Kenapa beda-beda tiap note type?"
    Kebanyakan note type hanya menyimpan satu kalimat per kartu, jadi kata yang sudah punya kartu cukup tidak ditambang lagi. Senren bisa menyimpan beberapa adegan dalam satu kartu, jadi kata yang sama justru perlu menambah adegan ke kartu lamanya. Karena itu pengaturan `Duplicates` dan `Update Mode` Senren paling berbeda.

---

## Isian per note type

=== "Lapis"

    `Duplicates`: nyalakan `Check for Duplicates`, lalu pilih `Prevent` di `Duplicate Action`. `Update Mode` bisa dibiarkan seperti bawaannya.

    | Field | Isi |
    |---|---|
    | Expression | `Target Word` |
    | ExpressionFurigana | `Custom Template`: `{furigana-plain}` |
    | ExpressionReading | `Reading` |
    | ExpressionAudio | `Word Audio` |
    | SelectionText | Kosong |
    | MainDefinition | `Single Glossary`, lalu pilih kamusnya |
    | DefinitionPicture | Kosong |
    | Sentence | `Sentence with Bold Word` |
    | SentenceFurigana | Kosong. **Wajib kosong**, kalau diisi kartunya bisa rusak |
    | SentenceAudio | `Sentence Audio` |
    | Picture | `Image` |
    | Glossary | `Glossary` |
    | Hint | Kosong |
    | IsWordAndSentenceCard, IsClickCard, IsSentenceCard, IsAudioCard | Kosong, kecuali kamu mau jenis kartu lain (lihat catatan di bawah) |
    | PitchPosition | `Pitch Accent Positions` |
    | PitchCategories | `Pitch Accent Categories` |
    | Frequency | `Frequencies` |
    | FreqSort | `Frequency Harmonic Rank` |
    | MiscInfo | `Media Name` |

    Kalau semua field `Is...Card` kosong, kartunya berupa kartu kosakata biasa. Untuk jenis kartu lain, pilih **satu** field `Is...Card` saja, isi dengan `Custom Template` berisi huruf `x`:

    - `IsWordAndSentenceCard`: kalimat muncul sebagai petunjuk di bawah kata
    - `IsClickCard`: kata bisa diklik untuk memunculkan kalimat
    - `IsSentenceCard`: kalimat lengkap muncul di depan kartu
    - `IsAudioCard`: audio kalimat diputar dan kalimatnya muncul tanpa kata yang dicari

    Sumber: [Lapis](https://github.com/donkuri/lapis)

=== "Kiku"

    Field Kiku sama dengan Lapis, jadi ikuti tab **Lapis**. Kiku punya dua field tambahan yang dibiarkan kosong:

    | Field | Isi |
    |---|---|
    | SentenceTranslation | Kosong |
    | RelatedExpression | Kosong |

    `Duplicates`: nyalakan `Check for Duplicates`, lalu pilih `Prevent` di `Duplicate Action`.

    Kiku juga bisa menggabungkan beberapa kalimat dan gambar ke satu kartu, tapi caranya berbeda dengan Senren dan diatur dari Anki. Detailnya ada di [Field Grouping Kiku](https://github.com/youyoumu/kiku/blob/main/apps/docs/mds/field-grouping.md).

    Sumber: [Kiku: Switching From Lapis](https://github.com/youyoumu/kiku/blob/main/apps/docs/mds/migration.md)

=== "Senren"

    Senren bisa menyimpan beberapa adegan (kalimat, gambar, dan audio) untuk satu kata, lalu kamu bisa berpindah adegan di kartunya. Supaya ini jalan, menambang kata yang sama harus menambah adegan ke kartu lama.

    `Duplicates`: nyalakan `Check for Duplicates`, lalu pilih `Overwrite` di `Duplicate Action`. Lalu isi `Update Mode` tiap field sesuai tabel.

    | Field | Isi | Update Mode |
    |---|---|---|
    | word | `Target Word` | `Overwrite if available` |
    | reading | `Reading` | `Overwrite if available` |
    | sentence | `Custom Template`: `<span class="group">{cloze-prefix}<span class="highlight">{cloze-body}</span>{cloze-suffix}</span>` | `Append` |
    | sentenceFurigana | `Custom Template`: `<span class="group">{sentence-furigana}</span>` | `Append` |
    | sentenceTranslation | Kosong | `Append` |
    | sentenceCard | Kosong | `Fill if empty` |
    | audioCard | Kosong | `Fill if empty` |
    | notes | Kosong | `Fill if empty` |
    | hint | Kosong | `Fill if empty` |
    | picture | `Image` | `Append` |
    | wordAudio | `Word Audio` | `Fill if empty` |
    | sentenceAudio | `Sentence Audio` | `Append` |
    | selectionText | `Custom Template`: `{popup-selection-text}` | `Fill if empty` |
    | definition | `Single Glossary`, lalu pilih kamusnya | `Fill if empty` |
    | glossary | `Glossary` | `Fill if empty` |
    | pitchAccents | `Pitch Accent` | `Overwrite if available` |
    | pitchPositions | `Pitch Accent Positions` | `Overwrite if available` |
    | pitchCategories | `Pitch Accent Categories` | `Overwrite if available` |
    | frequencies | `Frequencies` | `Overwrite if available` |
    | freqSort | `Frequency Harmonic Rank` | `Overwrite if available` |
    | miscInfo | `Media Name` | `Append` |
    | dictionaryPreference | Kosong | `Fill if empty` |

    - `<span class="group">` adalah penanda satu adegan. Jangan dihapus dari template `sentence` dan `sentenceFurigana`.
    - Tombol pindah adegan baru muncul kalau kartunya punya minimal dua audio kalimat.
    - `sentenceTranslation` diisi sendiri di Anki kalau kamu mau terjemahan kalimat. Bungkus tiap terjemahan dengan `<span class="group">...</span>` supaya ikut adegannya. Manatan tidak bisa mengambil teks dari clipboard seperti Yomitan.

    ??? info "Bedanya dengan pengaturan Senren di Yomitan <small>(klik di sini)</small>"

        Di Yomitan, `picture` dan `sentenceAudio` biasanya dikosongkan karena diisi oleh alat lain, misalnya asbplayer. Di Manatan, gambar dan audio kalimat diambil langsung oleh Manatan, jadi kedua field itu diisi `Image` dan `Sentence Audio` dengan `Append` supaya tiap adegan punya gambar dan audionya sendiri. Field lainnya sama dengan pengaturan Yomitan.

    Sumber: [Senren: scene switching](https://brenoaqua.github.io/Senren/scene_switching) dan [Senren Setup](https://brenoaqua.github.io/Senren/setup_overview/)

=== "Mining-JP"

    `Duplicates`: nyalakan `Check for Duplicates`, lalu pilih `Prevent` di `Duplicate Action`. `Update Mode` bisa dibiarkan seperti bawaannya.

    | Field | Isi |
    |---|---|
    | Expression | `Target Word` |
    | ExpressionFurigana | `Custom Template`: `{furigana-plain}` |
    | ExpressionReading | `Reading` |
    | ExpressionAudio | `Word Audio` |
    | MainDefinition | `Custom Template`: `{popup-selection-text}` |
    | Sentence | `Sentence with Bold Word` |
    | SentenceFurigana | Kosong |
    | SentenceAudio | `Sentence Audio` |
    | FullDefinition | `Glossary` |
    | Image | `Image` |
    | Translation | Kosong |
    | PitchPosition | `Pitch Accent Positions` |
    | Hint | Kosong |
    | Frequency | `Frequencies` |
    | FreqSort | `Frequency Harmonic Rank` |
    | MiscInfo | `Media Name` |
    | ExtraField | Kosong |
    | *IsSentenceCard | Kosong |

    `MainDefinition` diisi teks yang kamu sorot di popup, seperti saran pembuat note type ini. Kalau tidak menyorot apa pun, field ini kosong.

    Sumber: [JP-study (Mining-JP)](https://github.com/rudnam/JP-study)

---

## Kartu tidak sesuai?

- **Field kosong padahal sudah diisi:** cek lagi nama field di Anki. Huruf besar dan kecil harus sama persis, misalnya `sentence` di Senren berbeda dengan `Sentence` di Lapis.
- **Kalimat menumpuk di satu kartu (selain Senren):** `Duplicate Action` masih `Overwrite` dan field kalimat diatur `Append`. Ganti `Duplicate Action` ke `Prevent`.
- **Adegan baru di Senren menimpa adegan lama:** field `sentence`, `sentenceFurigana`, `sentenceAudio`, `picture`, atau `miscInfo` masih `Overwrite`. Ganti ke `Append`.
- **Muncul kartu baru untuk kata yang sama:** `Check for Duplicates` mati atau `Duplicate Action` diatur `Add anyway`.
