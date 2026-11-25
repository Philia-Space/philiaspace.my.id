# Panduan Gaya Penulisan Philia Space

Pegangan untuk siapa pun yang menulis atau menyunting halaman di `docs/`. Tujuannya satu: semua halaman terdengar seperti ditulis orang yang sama.

Contoh halaman yang sudah mengikuti gaya ini: [Panduan Bahasa Jepang](docs/panduan.md) untuk halaman bacaan, [Setup Fushi](docs/Setup-Fushi.md) untuk halaman tutorial.

## Nada dan sapaan

- Santai tapi rapi, seperti kakak tingkat yang menjelaskan ke adik tingkat. Tidak kaku, tapi juga bukan bahasa chat.
- Sapa pembaca dengan **kamu**. Jangan pakai "Anda", "kalian", atau "saya".
- Tidak ada narator "aku". Kalau sumber aslinya memakai sudut pandang penulis ("aku dulu juga..."), ubah jadi kalimat umum atau sebut sumbernya ("menurut TheMoeWay, ...").
- Kata santai boleh sesekali kalau memang lebih wajar: *nonton*, *ngobrol*, *bakal*. Jangan dijadikan gaya dasar.

| Hindari | Pakai |
|---|---|
| nggak, gak, ga | tidak (atau "bukan" sesuai konteks) |
| udah | sudah |
| kayak | seperti |
| banget | sangat, atau hapus kalau tidak perlu |
| aja | saja |
| buat (dalam arti "untuk") | untuk |
| ngerti, nyari, ngatur | mengerti, mencari, mengatur |
| temuin, hafalin | temukan, hafalkan |

## Istilah baku

| Pakai | Bukan | Catatan |
|---|---|---|
| unduh | download | |
| pasang | install, instal | Kalau nama tombolnya `Install`, tulis persis tombolnya: klik `Install` |
| perbarui, pembaruan | update | Sama: nama tombol tetap `Update` |
| pengaturan | setting, settings | Nama menu tetap `Settings` |
| ekstrak | extract, unzip | |
| klik, tekan | | "klik" untuk PC, "tekan" untuk HP |
| immersion | imersi | |
| kosakata | vocab | |
| tata bahasa | grammar, bunpou | "bunpou" boleh kalau sedang membahas istilah Jepangnya |
| kartu | card | "flashcard" boleh |
| dek | deck | Nama menu tetap `Deck` |
| ulasan | review | Untuk kartu Anki. *review hell* boleh dalam kurung |
| add-on | addon, addons | Nama folder tetap `addons21` |
| HP | ponsel, handphone | |

Nama aplikasi dan fitur ditulis seperti aslinya: Anki, Yomitan, AnkiConnect, Manatan, Fushi, note type, deck, mining. Tidak perlu diterjemahkan.

## Halaman tutorial

- Satu langkah satu tindakan. Mulai dengan kata kerja perintah: "Buka", "Klik", "Salin", "Pilih".
- Nama tombol, menu, dan field ditulis dengan backtick, persis seperti di layar (huruf besar kecilnya juga): `Tools` > `Add-ons` > `Get Add-ons...`
- Tombol keyboard pakai `++ctrl+shift+i++`: satu pasang `++` untuk seluruh kombinasi, supaya tanda "+" tampil di antara tombol. Jangan dipecah jadi `++ctrl++ + ++shift++ + I`. Panah ditulis `left`, `right`, `up`, `down`.
- Nama file dan folder pakai backtick: `addons21`, `C:\Users\NamaKamu\AppData\Roaming\Anki2`
- Langkah yang berbeda per sistem operasi pakai tab (`=== "Windows"`, `=== "MacOS"`), bukan paragraf "kalau Windows..., kalau Mac...".
- Info tambahan yang tidak wajib dibaca masuk ke kotak lipat (`??? info`), supaya langkah utamanya tetap pendek.

## Kalimat

- Satu kalimat satu gagasan. Kalimat yang lebih dari dua baris di layar biasanya bisa dipecah.
- Hindari pembuka basa-basi ("Nah, sekarang kita akan membahas..."). Langsung ke isinya.
- Hindari frasa terjemahan kaku: "di mana" sebagai kata sambung, "yang mana", "adalah merupakan", "melakukan instalasi" (cukup "pasang").
- Penekanan pakai **tebal**, secukupnya. Jangan HURUF BESAR semua.

## Bagian yang sama di banyak halaman

**Tanggal halaman** tidak perlu ditulis. Tanggal dibuat dan terakhir diperbarui muncul otomatis di bawah halaman, diambil dari riwayat git. Jangan tambahkan baris "Diunggah: … · Diperbarui: …" lagi.

**Kotak untuk halaman terjemahan TheMoeWay:**

```markdown
!!! info "Terjemahan dari TheMoeWay"
    Halaman ini terjemahan bahasa Indonesia dari [Judul halaman aslinya](https://learnjapanese.moe/...) di TheMoeWay, ditulis oleh **shoui** dan kontributor TheMoeWay. Sebagian referensi dan sumber belajar diganti ke versi bahasa Indonesia.

    Versi asli dan terjemahan ini sama-sama berlisensi [GPL-3.0](https://www.gnu.org/licenses/gpl-3.0.html). Kalau kamu nyaman baca bahasa Inggris, baca [versi aslinya](https://learnjapanese.moe/...).
```

**Kotak untuk halaman dari LazyGuide** (taruh tepat di bawah judul halaman). Pilih judul kotak sesuai kondisi halamannya:

- `Terjemahan dari LazyGuide`: isi dan urutan bagiannya mengikuti versi asli.
- `Diadaptasi dari LazyGuide`: berdasarkan versi asli, tapi ada bagian besar yang ditambah atau diganti. Sebut bagian apa saja di paragraf kedua.
- `Sebagian dari LazyGuide`: hanya sebagian kecil halaman yang diambil. Sebut bagian mana.

```markdown
!!! info "Terjemahan dari LazyGuide"
    Halaman ini terjemahan bahasa Indonesia dari [Judul halaman aslinya](https://lazyguidejp.github.io/jp-lazy-guide/...) di LazyGuide, ditulis oleh **LazyGuideJP**. Sebagian referensi dan sumber belajar diganti ke versi bahasa Indonesia.

    Versi aslinya berlisensi [MIT](https://github.com/LazyGuideJP/lazyguidejp.github.io/blob/main/LICENSE), halaman ini berlisensi GPL-3.0 (rinciannya di [lisensi Philia Space](https://github.com/Philia-Space/philiaspace.my.id/blob/main/LICENSE.docs.md)). Kalau kamu nyaman baca bahasa Inggris, baca [versi aslinya](https://lazyguidejp.github.io/jp-lazy-guide/...).
```

Kalau halaman baru diambil dari LazyGuide, tambahkan juga ke daftar di `LICENSE.docs.md`.

## Yang jangan diubah saat menyunting

- Alamat tautan, path gambar, isi blok kode, dan password arsip.
- Penanda `<!-- upstream: ... -->` di baris pertama halaman LazyGuide, atau tepat setelah front matter kalau halamannya punya front matter (front matter harus selalu di baris pertama). Urutan langkah dan judul bagian di halaman itu juga sebaiknya tetap sama dengan versi LazyGuide supaya mudah disinkronkan.
- Judul bagian yang dirujuk tautan `#...` dari halaman lain. Kalau judulnya terpaksa diganti, cari dan perbaiki semua tautan ke judul itu.

## Riwayat perubahan

Perubahan yang terasa oleh pembaca dicatat di [Riwayat Perubahan](docs/riwayat-perubahan.md). Penyuntingan bahasa saja cukup ditulis satu baris per halaman, misalnya "bahasa dirapikan agar lebih mudah dibaca", tanpa daftar kata yang diganti.

Satu tanggal cukup ditulis sekali. Tanggal terbaru di paling atas, tapi di dalam satu tanggal perubahan diurutkan dari yang paling awal, jadi perubahan baru ditulis di bawah perubahan terakhir tanggal itu:

```markdown
**16-11-2026**

*Judul perubahan pertama*

- Penambahan
       - ...

*Judul perubahan berikutnya*

- Perbaikan
       - ...
```
