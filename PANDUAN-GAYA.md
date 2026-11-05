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

**Baris tanggal** di bawah judul:

```markdown
Diunggah: 10 Agustus 2025 · Diperbarui: 5 November 2026 – `Yaaacha`
```

**Kotak untuk halaman terjemahan TheMoeWay:**

```markdown
??? warning "Perhatian <small>(klik di sini)</small>"
    - Panduan ini adaptasi dan lokalisasi dari [TheMoeWay](https://learnjapanese.moe/...), dengan referensi dan sumber belajar yang diganti ke versi bahasa Indonesia.
    - Kalau kamu nyaman baca panduan bahasa Inggris, versi aslinya ada di tautan itu.
```

## Yang jangan diubah saat menyunting

- Alamat tautan, path gambar, isi blok kode, dan password arsip.
- Penanda `<!-- upstream: ... -->` di baris pertama halaman LazyGuide. Urutan langkah dan judul bagian di halaman itu juga sebaiknya tetap sama dengan versi LazyGuide supaya mudah disinkronkan.
- Judul bagian yang dirujuk tautan `#...` dari halaman lain. Kalau judulnya terpaksa diganti, cari dan perbaiki semua tautan ke judul itu.

## Riwayat perubahan

Perubahan yang terasa oleh pembaca dicatat di [Riwayat Perubahan](docs/riwayat-perubahan.md). Penyuntingan bahasa saja cukup ditulis satu baris per halaman, misalnya "bahasa dirapikan agar lebih mudah dibaca", tanpa daftar kata yang diganti.
