# Setup Chimahon (Android)
---

 Diunggah: 6 November 2026 – `Yaaacha`

---

!!! warning "Draft"
    Halaman ini masih draft dan belum masuk menu. Langkahnya disusun dari kode sumber Chimahon v2.4.8 dan **belum dicoba langsung di HP**, jadi letak tombol bisa sedikit berbeda. Screenshot menyusul.

??? info "Info: tentang Chimahon <small>(klik di sini)</small>"

    Chimahon adalah aplikasi Android untuk membaca manga dan menonton anime sambil mencari kata dengan kamus popup, lalu mengirim katanya jadi kartu di AnkiDroid. Chimahon dibuat dari Mihon, jadi tampilannya mirip Mihon atau Tachiyomi.

    Di Philia Space, Chimahon dipakai untuk **anime dan manga** di HP. Untuk light novel, pakai [Hoshi Reader](Setup-Hoshi-Reader.md).

    Aplikasinya masih berbahasa Inggris. Di halaman ini nama tombol ditulis persis seperti yang muncul di layar.

---

## **Persiapan**

1. Unduh APK Chimahon dari [rilis terbaru di GitHub](https://github.com/Chimahon/chimahon/releases/latest). Buka bagian `Assets` kalau daftar filenya belum terlihat

    | File | Untuk |
    |---|---|
    | `chimahon-arm64-v8a-v….apk` | Hampir semua HP sekarang. Pilih ini kalau ragu |
    | `chimahon-armeabi-v7a-v….apk` | HP lama (32-bit) |
    | `chimahon-v….apk` | Semua jenis HP, ukurannya lebih besar |

    Chimahon butuh Android 8.0 ke atas.

2. Pasang [AnkiDroid](https://play.google.com/store/apps/details?id=com.ichi2.anki) dari Play Store
3. Siapkan dek dan note type Lapis di AnkiDroid. Cara paling mudah: ikuti [Setup Anki PC](setup-anki-pc-lazy-guide.md) di komputer, lalu masuk ke akun AnkiWeb yang sama di AnkiDroid dan tekan sinkron. `Mining Deck` dan note type `Lapis` akan ikut masuk ke HP
    - Kalau tidak punya PC, lewati langkah ini. Chimahon bisa membuat note type `Lapis` sendiri di AnkiDroid (lihat [Kartu Anki](#kartu-anki))
4. Unduh kamus format Yomitan (`.zip`) ke HP. Kamus yang sama dengan panduan lain bisa langsung dipakai
    - Kamus JP-ID
        - [JIDict](https://github.com/philiaspaceai/JIDict-yomitan#pemasangan)
        - [RH Dict](https://discord.com/channels/1370274344571240552/1544821080148025484/1544821080148025484) (di Discord Philia Space)
    - Kamus lain: pilih dari daftar rekomendasi di bawah

Daftar rekomendasinya sama dengan di [Setup Yomitan dan Anki PC](setup-yomitan-pc.md#kamus).

- [Koleksi Shoui](https://learnjapanese.link/dictionaries) dari TMW
- [Koleksi Marv](https://drive.google.com/drive/folders/1xURpMJN7HTtSLuVs9ZtIbE7MDRCdoU29) dari Yomitan

Kalau tidak ingin punya terlalu banyak kamus, pakai daftar ringkas di bawah.

??? info "Daftar Ringkas oleh [Donkuri](https://donkuri.github.io/learn-japanese/setup/#what-if-i-dont-want-to-use-all-these-dictionaries): <small>(klik di sini)</small>"

	<ul>
	  <li>JMdict (atau Jitendex)</li>
	  <li>JMnedict</li>
	  <li>三省堂 8th Ed (atau 明鏡 2nd Ed)</li>
	  <li>Kanji Jitenon</li>
	  <li>NHK2016</li>
	  <li>JPDB Frequency v2.2</li>
	</ul>

Di bawah ini ada beberapa rekomendasi yang bisa kamu pilih. Kamu bisa mencampurnya atau mengikuti semuanya, sesuai keinginan.

<details>
<summary><b>Daftar Rekomendasi <i>shoui</i> dari TheMoeWay (TMW):</b> <i>(klik di sini)</i></summary>

<p><b>Bilingual</b></p>
<ul>
  <li>[Bilingual] JMdict Extra (Recommended).zip</li>
  <li>[Bilingual] 新和英.zip</li>
</ul>

<p><b>Frekuensi</b></p>
<ul>
  <li>[Freq] CC100.zip</li>
  <li>[Freq] JPDB (Recommended).zip</li>
</ul>

<p><b>Kanji</b></p>
<ul>
  <li>[Kanji] KANJIDIC (English) (Recommended).zip</li>
</ul>

<p><b>Monolingual</b></p>
<ul>
  <li>[Monolingual] 実用日本語表現辞典 (Recommended).zip</li>
  <li>[Monolingual, Encyclopedia] PixivLight.zip</li>
</ul>

<p><b>Tata Bahasa</b></p>
<ul>
  <li>[Grammar] Dictionary of Japanese Grammar 日本語文法辞典 (Recommended).zip</li>
  <li>[Grammar] どんなとき使う日本語表現文型辞典.zip</li>
  <li>[Grammar] 毎日のんびり日本語教師 (nihongosensei).zip</li>
  <li>[Grammar] JLPT文法解説まとめ(nihongo_kyoushi).zip</li>
  <li>[Grammar] 絵でわかる日本語.zip</li>
</ul>

<p><b>Nama</b></p>
<ul>
  <li>[Names] JMnedict.zip</li>
</ul>

<p><b>Pitch</b></p>
<ul>
  <li>[Pitch] アクセント辞典v2 (Recommended).zip</li>
</ul>

</details>

<details>
<summary><b>Daftar Rekomendasi <i>marv</i> dari Yomitan:</b> <i>(klik di sini)</i></summary>

<p><b>Bilingual</b></p>
<ul>
  <li>[JA-EN] jitendex-yomichan</li>
  <li>[JA-EN] NEW 斎藤和英大辞典</li>
  <li>[JA-EN] 新和英</li>
</ul>

<p><b>Tata Bahasa</b></p>
<ul>
  <li>[JA Grammar] dojg-consolidated-v1_01</li>
</ul>

<p><b>Frekuensi</b></p>
<ul>
  <li>[JA Freq] JPDB_2022-05-10T03_27_02.930Z</li>
  <li>[JA Freq] Freq_CC100</li>
  <li>[JA Freq] BCCWJ-LUW</li>
</ul>

<p><b>Monolingual</b></p>
<ul>
  <li>[JA-JA] 実用日本語表現辞典</li>
  <li>[JA-JA] デジタル大辞泉</li>
  <li>[JA-JA Encyclopedia] Pixiv</li>
</ul>

<p><b>Kanji</b></p>
<ul>
  <li>[Kanji] KANJIDIC_english</li>
  <li>[Kanji] JPDB Kanji</li>
</ul>

<p><b>Pitch Accent</b></p>
<ul>
  <li>[Pitch] 大辞泉</li>
</ul>

</details>

<details>
<summary><b>Daftar Kamus Pilihan Yaaacha:</b> <i>(klik di sini)</i></summary>

<p><b>Kamus Bilingual</b></p>
<ul>
  <li>1. JIDict<br>   Kamus Jepang-Indonesia berbasis JMdict dan Sanseido, dikembangkan oleh tim Philia Space, berfokus pada hasil yang mudah dipahami pelajar bahasa Jepang di Indonesia.</li>
  <li>2. JMdict<br>   Kamus Jepang-Inggris utama dengan lebih dari 180.000 entri. Banyak dipakai sebagai sumber utama kamus turunan lain. Secara bawaan sudah terhubung dengan Yomitan, jadi pembaruannya bisa dicek langsung di menu <code>Dictionaries</code>.</li>
  <li>3. Jitendex.org<br>   Versi gabungan dari kamus bilingual JMdict, dengan tambahan fitur khusus dari situs Jitendex.org. Secara bawaan sudah terhubung dengan Yomitan, jadi pembaruannya bisa dicek langsung di menu <code>Dictionaries</code>.</li>
  <li>4. 新和英<br>   Kamus Jepang-Inggris resmi dari Kenkyusha, dengan definisi yang lebih formal dan kontekstual dibanding JMdict.</li>
</ul>

<p><b>Kamus Nama & Kanji</b></p>
<ul>
  <li>5. JMnedict<br>   Kamus nama orang, tempat, dan organisasi dalam bahasa Jepang. Berguna saat menemukan nama khusus. Secara bawaan sudah terhubung dengan Yomitan, jadi pembaruannya bisa dicek langsung di menu <code>Dictionaries</code>.</li>
  <li>6. KANJIDIC (English)<br>   Informasi karakter kanji dalam bahasa Inggris, termasuk makna, bacaan, stroke, dan level JLPT. Secara bawaan sudah terhubung dengan Yomitan, jadi pembaruannya bisa dicek langsung di menu <code>Dictionaries</code>.</li>
  <li>7. 漢字源<br>   Kamus kanji berbahasa Jepang dengan penjelasan etimologi dan penggunaan historis. Lebih cocok untuk pembelajar lanjutan.</li>
  <li>8. weblio 古語辞典<br>   Kamus kosakata klasik Jepang. Membantu memahami bahasa kuno yang sering muncul dalam sastra dan sejarah.</li>
</ul>
<p><b>Monolingual – Kamus Besar & Onomatope</b></p>
<ul>
  <li>9. 旺文社国語辞典 第十一版<br> Kamus modern dengan definisi yang mudah dipahami, cocok untuk pelajar bahasa Jepang tingkat menengah.</li>
  <li>10. 明鏡国語辞典 第三版<br> Menyediakan definisi dengan gaya penjelasan yang jernih dan mudah dibaca.</li>
  <li>11. デジタル大辞泉<br> Kamus komprehensif modern yang sering digunakan oleh penutur asli.</li>
  <li>12. 岩波国語辞典 第八版<br> Kamus yang terkenal dengan keakuratan dan gaya konservatifnya.</li>
  <li>13. 広辞苑 第七版<br> Salah satu kamus Jepang terbesar dan paling prestisius.</li>
  <li>14. 精選版 日本国語大辞典<br> Versi ringkas dari 日本国語大辞典, tetap komprehensif namun lebih praktis.</li>
  <li>15. ハイブリッド新辞林<br> Gabungan dari berbagai sumber, cepat dan ringan untuk pencarian harian.</li>
  <li>16. 新明解国語辞典 第八版<br> Dikenal karena penjelasan yang berani dan interpretatif.</li>
  <li>17. 三省堂国語辞典 第八版<br> Kamus ringkas namun mendalam, sangat cocok untuk pengguna tingkat menengah.</li>
  <li>18. 例解学習国語辞典 第十一版<br> Kamus anak-anak yang sangat ramah pelajar asing.</li>
  <li>19. 新選国語辞典 第十版<br> Kamus ringkas untuk referensi cepat.</li>
  <li>20. 国語辞典オンライン<br> Versi daring ringan yang berisi banyak entri praktis.</li>
  <li>21. 実用日本語表現辞典<br> Fokus pada ekspresi praktis dan idiom.</li>
  <li>22. surasura 擬声語<br> Khusus kosakata onomatope, lengkap dengan contoh penggunaan dan makna.</li>
</ul>
<p><b>Kamus Tata Bahasa & Pelajaran:</b></p>
<ul>
  <li>23. 日本語文法辞典（全集）<br> Seri lengkap kamus tata bahasa DoJG (Beginner–Advanced) dalam format yang bisa dicari.</li>
  <li>24. JLPT文法解説まとめ<br> Ringkasan tata bahasa JLPT dari berbagai sumber, mudah ditelusuri.</li>
  <li>25. 毎日のんびり日本語教師<br> Penjelasan tata bahasa yang ringan dan jelas, dengan label level JLPT.</li>
  <li>26. 絵でわかる日本語<br> Kamus tata bahasa berbasis ilustrasi, cocok untuk pemula dan yang lebih mudah belajar lewat gambar.</li>
</ul>

<p><b>Kamus Pendukung (3 kanji atau lebih):</b></p>
<ul>
  <li>27. 学研 四字熟語辞典<br> Fokus pada idiom empat kanji, termasuk makna dan contoh penggunaan.</li>
  <li>28. 新明解四字熟語辞典<br> Alternatif dengan definisi yang unik dan gaya khas 新明解.</li>
</ul>

<p><b>Kamus Khusus (dialek, peribahasa, dan sejenisnya):</b></p>
<ul>
  <li>29. 故事ことわざの辞典<br>Berisi peribahasa dan ungkapan klasik Jepang.</li>
  <li>30. 故事・ことわざ・慣用句オンライン<br>Versi daring dari berbagai sumber idiomatik.</li>
  <li>31. ことわざ・慣用句の百科事典<br>Ensiklopedia idiom dan ungkapan tetap (set phrases).</li>
  <li>32. 全国方言辞典<br>Kamus dialek dari berbagai daerah Jepang.</li>
</ul>

<p><b>Kamus JLPT, Frekuensi & Korpus:</b></p>
<ul>
  <li>33. JLPT<br>Kumpulan kosakata JLPT level N1–N5.</li>
  <li>34. CC100<br>Korpus bahasa Jepang yang digunakan untuk analisis frekuensi kata.</li>
  <li>35. JPDB<br>Frekuensi kosakata dari database JPDB.</li>
  <li>36. YouTube<br>Frekuensi kata berdasarkan subtitle video YouTube Jepang.</li>
  <li>37. BCCWJ<br>Balanced corpus of contemporary written Japanese (BCCWJ).</li>
  <li>38. PixivLight<br>Frekuensi kosakata dari karya buatan pengguna di Pixiv.</li>
</ul>

<p><b>Kamus Pitch Accent:</b></p>
<ul>
  <li>39. 大辞林第四版<br>Selain kamus besar, versi ini menyertakan informasi pitch accent.</li>
  <li>40. 三省堂国語辞典第八版 (pitch)<br>Tambahan aksen dari 三省堂 untuk entri tertentu.</li>
  <li>41. 新明解第八版 (pitch)<br>Informasi pitch berdasarkan edisi 新明解 ke-8.</li>
  <li>42. 大辞泉 (pitch)<br>Pitch accent versi tambahan untuk entri 大辞泉.</li>
  <li>43. アクセント辞典<br>Kamus aksen khusus untuk penutur asli dan pembelajar tingkat lanjut.</li>
  <li>44. NHK 日本語発音アクセント新辞典<br>Standar referensi aksen NHK untuk kata-kata Jepang modern.</li>
  <li>45. NHK (pitch)<br>Tambahan pitch untuk entri berdasarkan standar NHK.</li>
</ul>

</details>

---

## **Pasang**

1. Buka file APK yang tadi diunduh
2. Kalau muncul peringatan aplikasi dari sumber tidak dikenal, tekan `Settings`, nyalakan izin untuk browser atau file manager yang kamu pakai, lalu kembali dan tekan `Install`
3. Buka Chimahon. Ikuti layar pembuka sampai masuk ke halaman utama
4. Saat diminta memilih **folder penyimpanan** (`Storage location`), buat atau pilih folder khusus, misalnya `Chimahon` di memori internal. Folder ini dipakai untuk backup, unduhan, dan file manga/anime lokal

    Kalau terlewat, atur nanti di `More` > `Settings` > `Data and storage` > `Storage location`.

---

## **Kamus**

1. Buka `More` > `Settings` > `Dictionaries and audio`
2. Di bagian `Imported dictionaries`, tekan `Import dictionary`, lalu pilih file `.zip` kamus. Beberapa file bisa dipilih sekaligus, dan file `.zip` **tidak perlu diekstrak**
3. Tunggu sampai muncul laporan `Imported successfully`
4. Atur urutan kamus. Kamus paling atas tampil paling dulu. Kalau ingin arti bahasa Indonesia muncul duluan, taruh JIDict di urutan pertama

Ukuran dan tampilan popup kamus bisa diatur di `More` > `Settings` > `Popup dictionary`.

---

## **Kartu Anki**

Pastikan AnkiDroid sudah terpasang dan pernah dibuka sekali.

1. Buka `More` > `Settings` > `Anki`
2. Nyalakan `Enable Anki integration`. Saat AnkiDroid meminta izin, tekan izinkan
3. Di `Default deck`, pilih `Mining Deck` (atau dek lain yang kamu pakai untuk mining)
4. Di `Note type`, pilih `Lapis`. Kalau `Lapis` belum ada di AnkiDroid, Chimahon menambahkannya sendiri
5. Buka `Field mapping` dan pastikan field Lapis sudah terisi. Untuk `Lapis`, Chimahon mengisinya otomatis
6. (Opsional) Di `When duplicate found`, pilih `Don't add` supaya kata yang sudah ada di dek tidak dibuat dua kali

Sekarang setiap kata yang kamu cari punya tombol untuk dijadikan kartu. Kartu langsung masuk ke AnkiDroid.

---

## **Manga**

### **Siapkan file manga**

Chimahon membaca manga dari folder `local` di dalam folder penyimpanan tadi. Satu judul satu folder, satu chapter atau volume satu file `.cbz` atau `.zip`:

```
Chimahon/
└── local/
    └── Yotsubato/
        ├── Volume 01.cbz
        ├── Volume 01.mokuro
        ├── Volume 02.cbz
        └── Volume 02.mokuro
```

- Kalau kamu sudah memproses manga dengan Mokuro (lihat [Setup Manga PC](setup-manga-pc-lazy-guide.md)), taruh file `.mokuro` di sebelah file manganya dengan **nama yang sama**. Untuk manga berupa folder gambar, taruh file `.mokuro` di dalam folder itu. Teks hasil OCR langsung bisa dipakai tanpa proses ulang
- Kalau tidak punya file `.mokuro`, Chimahon bisa membaca teks halaman sendiri (lihat [OCR di HP](#ocr-di-hp))

Bisa juga tanpa menyalin ke folder `local`: di tab `Browse` > `Sources`, tekan ikon `+`, lalu pilih folder gambar atau file `.cbz` manganya.

### **Baca dan mining**

1. Buka tab `Browse`, lalu pilih `Local source`
2. Pilih judul manga, lalu buka chapter atau volumenya
3. Buka menu di dalam pembaca, lalu tekan `Enable OCR`. Langkah ini tetap perlu walaupun manganya sudah punya file `.mokuro`
4. Tekan teks di balon dialog untuk membuka popup kamus
5. Tekan tombol tambah kartu di popup untuk mengirim kata ke Anki

### **OCR di HP**

Untuk manga tanpa file `.mokuro`, `Enable OCR` membuat Chimahon membaca teks setiap halaman sendiri.

!!! warning "Mesin OCR bawaan memakai Google Lens"
    Pengaturan bawaan `OCR Engine` adalah `Cloud (Google Lens)`, artinya halaman manga dikirim ke Google untuk dibaca. Kalau tidak mau, buka `More` > `Settings` > `OCR` > `OCR Engine`, lalu pilih `Local (On-Device)`. Pilihan ini mengunduh model OCR dulu, berjalan tanpa internet, tapi lebih berat untuk baterai.

---

## **Anime**

### **Siapkan file anime**

Sama seperti manga, anime dibaca dari folder `localanime`. Taruh file subtitle Jepang di sebelah file videonya dengan **nama yang sama**, supaya subtitle terbuka otomatis:

```
Chimahon/
└── localanime/
    └── Yotsubato/
        ├── Episode 01.mkv
        ├── Episode 01.srt
        ├── Episode 02.mkv
        └── Episode 02.srt
```

Subtitle Jepang bisa diunduh di [Jimaku](https://jimaku.cc/).

### **Tonton dan mining**

1. Buka anime dari `Local anime` di tab `Browse`
2. Saat video berjalan, tekan kata di subtitle untuk membuka popup kamus
3. Tekan tombol tambah kartu di popup. Kartu dikirim lengkap dengan cuplikan layar dan audio kalimatnya

??? info "Cari subtitle Jimaku langsung dari Chimahon <small>(klik di sini)</small>"
    Chimahon bisa mencari dan mengunduh subtitle Jimaku tanpa keluar aplikasi, tapi butuh API key dari akun Jimaku-mu sendiri.

    1. Masuk ke [Jimaku](https://jimaku.cc/), lalu buat API key di halaman akunmu
    2. Di Chimahon, buka `More` > `Settings` > `Player` > `Subtitles`, lalu tempel API key-nya di `Jimaku API key`
    3. Saat menonton, buka daftar subtitle di pemutar, lalu tekan `Search Jimaku`

---

## **Pertanyaan Umum**

#### Pertanyaan 1: Bagaimana kalau belum pakai Anki?

Lewati bagian [Kartu Anki](#kartu-anki). Kamus popup tetap bisa dipakai untuk mencari kata.

#### Pertanyaan 2: Bagaimana dengan light novel?

Chimahon punya pembaca EPUB, tapi untuk light novel Philia Space menyarankan [Hoshi Reader](Setup-Hoshi-Reader.md) karena fiturnya lebih lengkap untuk membaca buku.
