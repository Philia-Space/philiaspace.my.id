# Setup Hoshi Reader (Android)
---

 Diunggah: 6 November 2026 – `Yaaacha`

---

!!! warning "Draft"
    Halaman ini masih draft dan belum masuk menu. Langkahnya disusun dari kode sumber Hoshi Reader Android v1.4.0 dan **belum dicoba langsung di HP**, jadi letak tombol bisa sedikit berbeda. Screenshot menyusul.

??? info "Info: tentang Hoshi Reader <small>(klik di sini)</small>"

    Hoshi Reader adalah aplikasi untuk membaca light novel dan buku EPUB sambil mencari kata dengan kamus popup, lalu mengirim katanya jadi kartu di AnkiDroid. Semuanya dalam satu aplikasi, tanpa perlu browser, Yomitan, atau AnkiConnect Android.

    Di Philia Space, Hoshi Reader dipakai untuk **light novel dan buku** di HP. Untuk anime dan manga, pakai [Chimahon](Setup-Chimahon.md).

    Hoshi Reader aslinya aplikasi iPhone. Versi Android ini dibuat ulang oleh komunitas dan isinya sudah setara dengan versi iPhone. Aplikasinya masih berbahasa Inggris, jadi nama tombol ditulis persis seperti yang muncul di layar.

??? info "Pakai iPhone atau iPad? <small>(klik di sini)</small>"

    Ikuti [Setup Hoshi Reader (iOS)](Setup-Hoshi-Reader-iOS.md). Cara membuat kartu Anki di iPhone berbeda dengan Android.

---

## **Persiapan**

1. Unduh APK Hoshi Reader dari [rilis terbaru di GitHub](https://github.com/HuangAntimony/Hoshi-Reader-Android/releases/latest). Buka bagian `Assets` kalau daftar filenya belum terlihat

    | File | Untuk |
    |---|---|
    | `Hoshi-Reader-v…-arm64-v8a.apk` | Hampir semua HP sekarang. Pilih ini kalau ragu |
    | `Hoshi-Reader-v…-armeabi-v7a.apk` | HP lama (32-bit) |

    Hoshi Reader butuh Android 8.0 ke atas.

2. Pasang [AnkiDroid](https://play.google.com/store/apps/details?id=com.ichi2.anki) dari Play Store
3. Siapkan dek dan note type Lapis di AnkiDroid. Ikuti [Setup Anki PC](setup-anki-pc-lazy-guide.md) di komputer, lalu masuk ke akun AnkiWeb yang sama di AnkiDroid dan tekan sinkron. `Mining Deck` dan note type `Lapis` akan ikut masuk ke HP
    - Kalau tidak punya PC, unduh [`Lapis.apkg`](https://github.com/donkuri/lapis/releases/latest) di HP, lalu buka filenya dengan AnkiDroid untuk mengimpornya
4. Unduh kamus format Yomitan (`.zip`) ke HP. Kamus yang sama dengan panduan lain bisa langsung dipakai
    - Kamus JP-ID
        - [JIDict](https://github.com/philiaspaceai/JIDict-yomitan#pemasangan)
        - [RH Dict](https://discord.com/channels/1370274344571240552/1544821080148025484/1544821080148025484) (di Discord Philia Space)
    - Kamus JP-EN bisa diunduh langsung dari dalam Hoshi Reader (lihat [Kamus](#kamus))
5. Siapkan file EPUB light novel di HP

---

## **Pasang**

1. Buka file APK yang tadi diunduh
2. Kalau muncul peringatan aplikasi dari sumber tidak dikenal, tekan `Settings`, nyalakan izin untuk browser atau file manager yang kamu pakai, lalu kembali dan tekan `Install`
3. Buka Hoshi Reader. Menu utamanya ada di bawah: `Books`, `Dictionary`, `Statistics`, dan `Settings`

---

## **Kamus**

1. Buka `Settings` > `Dictionaries`
2. Tekan ikon `+` di kanan atas, lalu pilih file `.zip` kamus. File `.zip` **tidak perlu diekstrak**
3. Untuk kamus JP-EN, tekan `Download Recommended Dictionaries`, lalu pilih kamus dari daftar. Hoshi Reader akan mengunduh dan memasangnya sendiri
4. Atur urutan kamus. Kamus paling atas tampil paling dulu. Kalau ingin arti bahasa Indonesia muncul duluan, taruh JIDict di urutan pertama

!!! tip "HP dengan RAM kecil"
    Kalau RAM HP-mu di bawah 3 GB dan impor kamus gagal atau aplikasinya tertutup sendiri, nyalakan `Low Memory Usage Mode` di halaman yang sama, lalu impor ulang.

**Cek kamus sudah jalan:** buka tab `Dictionary`, ketik kata Jepang, lalu lihat apakah artinya muncul.

---

## **Kartu Anki**

Pastikan AnkiDroid sudah terpasang dan pernah dibuka sekali.

1. Buka `Settings` > `Anki`
2. Tekan `Fetch` untuk mengambil daftar dek dan note type dari AnkiDroid. Saat AnkiDroid meminta izin, tekan izinkan
3. Di `Deck`, pilih `Mining Deck` (atau dek lain yang kamu pakai untuk mining)
4. Di `Model`, pilih `Lapis`
5. Buka `Fields` dan pastikan field Lapis sudah terisi. Untuk note type bernama `Lapis`, Hoshi Reader mengisinya otomatis
6. (Opsional) Nyalakan `Sync AnkiDroid after adding card` kalau mau kartu baru langsung tersinkron ke AnkiWeb

!!! warning "Biarkan `Use AnkiConnect` mati"
    Hoshi Reader membuat kartu langsung lewat AnkiDroid, jadi AnkiConnect Android tidak dibutuhkan. Kalau `Use AnkiConnect` dinyalakan tanpa diatur dengan benar, dek dan note type tidak bisa dimuat.

---

## **Membaca dan Mining**

1. Buka tab `Books`, lalu tekan `Import EPUB` dan pilih file EPUB-nya. Untuk banyak buku sekaligus, pakai `Import folder`
2. Tekan sampul buku untuk mulai membaca
3. Tekan kata yang tidak kamu tahu untuk membuka popup kamus. Kata di dalam arti kamus juga bisa ditekan untuk dicari lagi
4. Tekan tombol tambah kartu di popup untuk mengirim kata ke Anki. Kalimat tempat kata itu muncul ikut masuk ke kartu

Halaman bisa dibalik dengan tombol volume. Tampilan teks (vertikal atau horizontal, ukuran, font, tema) dan ukuran popup kamus diatur lewat tombol pengaturan di kanan bawah pembaca.

---

## **Audio Lokal**

Tanpa audio lokal, audio pengucapan diambil dari internet. Dengan audio lokal, audio tetap ada walaupun sedang offline, dan tidak perlu AnkiConnect Android.

!!! warning "Butuh ruang kosong sekitar 6 GB"
    File audionya sekitar 5,8 GB. Pastikan memori HP masih cukup sebelum impor.

1. Unduh [android.db](https://drive.google.com/file/d/1Fn11_nN04zM89yKFYBWVTi0Xpaf6I3qe/view)
2. Buka `Settings` > `Advanced` > `Audio`
3. Nyalakan `Local Audio`, tekan `Import`, lalu pilih file `android.db`

Hoshi Reader akan menambahkan sumber audio `Local` dan memakainya lebih dulu dibanding sumber lain.

---

## **Info Tambahan**

#### Info 1: Lanjut baca di PC

Hoshi Reader bisa menyinkronkan buku dan posisi baca lewat Google Drive, dengan format yang sama seperti ッツ Reader. Pengaturannya butuh membuat kunci akses Google Cloud sendiri, jadi lewati saja kalau hanya membaca di HP.

#### Info 2: Audiobook

Kalau punya audiobook dan subtitle-nya, Hoshi Reader bisa memutar audio sambil menandai kalimat yang sedang dibacakan dan membalik halaman sendiri. Untuk fitur yang sama di PC, lihat [Yatsu Whispersync](setup-LN-pc-lazy-guide.md#info-3-audiobook-dengan-yatsu-whispersync).

---

## **Pertanyaan Umum**

#### Pertanyaan 1: Apakah masih perlu Yomitan dan AnkiConnect Android?

Tidak. Kamus dan pembuatan kartu sudah ada di dalam Hoshi Reader. Panduan [LN & Buku Android](setup-LN-android-lazy-guide.md) yang memakai browser tetap bisa dipakai sebagai alternatif.
