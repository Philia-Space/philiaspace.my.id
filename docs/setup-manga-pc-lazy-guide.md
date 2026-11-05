<!-- upstream: setupMangaOnPC @ 2026-03-25 -->
# Setup Mining Manga di PC Windows [Lazy Guide](https://lazyguidejp.github.io/jp-lazy-guide/setupMangaOnPC/) 
---

 Diunggah: 24 Agustus 2025 · Diperbarui: 5 November 2026 – `Yaaacha`

---

- [OCR](setup-manga-pc-lazy-guide.md/#setup-ocr) adalah alat untuk scan teks Jepang di layar dan langsung menyimpan hasilnya ke clipboard, supaya bisa kamu cari dengan Yomitan.

- (Disarankan) [Mokuro Manga](setup-manga-pc-lazy-guide.md/#setup-mining-mokuro-manga) memproses manga lebih dulu supaya kamu bisa mengarahkan kursor ke kata-katanya dan langsung mencarinya dengan Yomitan.

---

## OCR

**Kebutuhan:**

- Pasang [CDisplayEx](https://www.cdisplayex.com/desktop/)  
    - Pembaca manga untuk PC
- [Yomitan di PC](setup-yomitan-pc-lazy-guide.md) dan [ShareX](setup-ShareX-pc.md) sudah terpasang dan diatur

---

## Setup OCR

1. Unduh [Python](https://www.python.org/downloads/release/python-3139/) (**baru diuji di versi 3.13.9**)  
    - Gulir ke bawah, pilih `Windows installer (64-bit)`, lalu pasang  
    - Centang `Add Python to PATH`

    ![Add Python to PATH](img/add-python-to-path.png){height=300 width=600}

2. Buka Command Prompt: tekan tombol Windows atau buka pencarian, lalu ketik `cmd`

3. Ketik `pip install owocr[mangaocr,screenai,lens]`  
    - Tunggu sampai pemasangan selesai (beberapa menit)  
    - Kalau muncul error `pip3 is not recognized...`:
        - Hapus (uninstall) Python, restart PC, lalu pasang lagi Python seperti di langkah 1. Ulangi kalau masih error (memang agak merepotkan)

4. Di [ShareX](setup-ShareX-pc.md), buka `Hotkey Settings` > `OCR (manga_ocr)` > klik ikon gir > `override screenshot folder`, lalu ganti path-nya ke folder OCR yang kamu mau

    ![ShareX OCR Path](img/sharex-ocr-path.png){height=150 width=300}

5. Di Command Prompt, ketik:
    - `owocr -e screenai -w clipboard -j -d -r "\path\to\sharex\screenshot\folder"`  
        - Ganti `path` dengan folder OCR yang kamu atur di langkah 4, lalu kecilkan (minimize) jendelanya
    - Bisa juga cukup ketik `owocr` tanpa path. Dengan cara ini, owocr akan scan dari mana saja
    - Kalau mau membuat shortcut program, lihat [Info 1](setup-manga-pc-lazy-guide.md/#info-1-shortcut-program-ocr)

6. Untuk scan, ambil gambar dengan hotkey ++shift+alt+q++ (atau hotkey OCR yang kamu atur di ShareX)  
    - Pastikan [Yomitan Search Page](setup-manga-pc-lazy-guide.md/#__tabbed_1_1) sudah terbuka  
    - Kalau mau scan dengan tombol mouse, lihat [Info 2](setup-manga-pc-lazy-guide.md/#info-2-scan-pakai-tombol-mouse)

7. Sekarang kamu sudah bisa mulai membaca manga dengan OCR
    - Engine bawaannya adalah (j) Screen AI (Google Lens lokal). Untuk mengganti engine, tekan tombol berikut di jendela Command Prompt: (l) Google Lens (online), (m) atau (n) MangaOCR, (b) Bing

    ??? info "Video Cara Pakai <small>(klik di sini)</small>"
        <iframe width="560" height="315" src="https://user-images.githubusercontent.com/22717958/150238361-052b95d1-0152-485f-a441-48a957536239.mp4" title="MangaOCR How-to" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

    === "Yomitan Search Page"
        ![Anki | Dark](img/yomitan-search-page.png){height=300 width=600}
    === "CDisplayEx Manga"
        ![Anki | Light](img/cdisplay-manga.png){height=300 width=600}

Kalau mau mencoba metode lain, lihat [Mokuro Manga](setup-manga-pc-lazy-guide.md/#setup-mining-mokuro-manga).

---

## Setup Mining Mokuro Manga

Ada 3 metode yang bisa dipilih:

- [Metode Instan](setup-manga-pc-lazy-guide.md/#metode-instan): tinggal impor, lalu langsung baca manga
- [Metode Online](setup-manga-pc-lazy-guide.md/#metode-online): memproses ±200 halaman manga dalam ±15 menit. Mudah, cukup ikuti panduannya
- [Metode Lokal](setup-manga-pc-lazy-guide.md/#metode-lokal): lebih bagus kalau PC kamu kuat, cocok untuk yang sudah paham hal teknis

!!! note "Mining di Android"
    Kalau mau mining di Android, lihat [Setup Manga di Android](setup-manga-android-lazy-guide.md)

---

### Metode Instan

1. Buka [Katalog Mokuro](https://catalog.mokuro.moe/).

2. Cari manga pilihanmu, pilih volume yang mau dibaca, lalu impor.

3. Tunggu sampai manga selesai diimpor.

4. Buka bagian [Baca Manga yang Sudah Diproses](setup-manga-pc-lazy-guide.md/#baca-manga-yang-sudah-diproses), ikuti langkah 1, lalu lompat ke langkah 3.

---

### Metode Online

1. Ikuti [panduan ini](https://colab.research.google.com/drive/1k-M1zr4hBnZTxlRODtNFn9r08XS5bKYB?usp=sharing)

2. Unduh folder manga yang sudah diproses, lalu lanjut ke [Baca Manga yang Sudah Diproses](setup-manga-pc-lazy-guide.md/#baca-manga-yang-sudah-diproses)

---

### Metode Lokal

1. Unduh [Python](https://www.python.org/downloads/release/python-3139/) (**baru diuji di versi 3.13.9**)  
    - Gulir ke bawah, pilih `Windows installer (64-bit)`, lalu pasang  
    - Centang `Add Python to PATH`
    ![Add Python to PATH](img/add-python-to-path.png){height=300 width=600}

2. Unduh dan pasang [Git](https://git-scm.com/downloads) (pilih 64-bit)

3. Buka Command Prompt: tekan tombol Windows atau buka pencarian, lalu ketik `cmd`

4. Ketik `pip3 install mokuro`
    - Tunggu beberapa menit sampai proses unduh dan pemasangan selesai dan kamu bisa mengetik lagi
    - Kalau muncul `pip3 is not recognized...`:
        - Hapus (uninstall) Python, restart PC, lalu pasang ulang Python seperti di langkah 1. Ulangi kalau masih gagal (memang merepotkan)

5. (Opsional) Pakai GPU dengan CUDA
    - Cek dulu apakah GPU kamu [mendukung CUDA](https://developer.nvidia.com/cuda-gpus)
    - Unduh [CUDA Toolkit](https://developer.nvidia.com/cuda-toolkit-archive) sesuai OS dan versimu
    - Ketik `pip3 install torch torchvision --index-url https://download.pytorch.org/whl/cu126` di `cmd` (atau cari perintah untuk versi terbaru [di sini](https://pytorch.org/get-started/locally/))

    ![Installing Torch](img/installing-torch.png){height=300 width=600}

    - Untuk mengecek apakah sudah terpasang, ketik `python` > `import torch` > `torch.cuda.is_available()`

        ![Torch if available](img/torch-if-available.png){height=150 width=300}

    - Kalau yang terbuka malah Microsoft Store:  
        - Buka `Windows Powershell`, tempel `Remove-Item $env:USERPROFILE\AppData\Local\Microsoft\WindowsApps\python*.exe`, lalu tekan ++enter++
    - Kalau ada masalah, pasang ulang PyTorch: hapus dulu dengan `pip uninstall torch` di `cmd`, lalu ulangi langkah di atas. Kalau masih gagal, lihat cara verifikasi lain [di sini](https://pytorch.org/get-started/locally/#windows-verification)

6. Ada dua cara memproses manga. Buka `cmd`, lalu:
    - Semua volume sekaligus:
        - Tempel: `mokuro --parent_dir F:\Manga\Saenai`
            - Ganti dengan path lengkap foldermu, dan "Saenai" dengan nama manga kamu
            - Folder Vol1, Vol2, Vol3, dan seterusnya harus ada di dalam folder `Saenai`, dengan pola nama yang seragam dan urut naik
    - Satu volume tertentu:
        - Tempel: `mokuro F:\Manga\Saenai\Vol3`
            - Ganti dengan path lengkap foldermu, "Saenai" dengan nama manga kamu, dan "Vol3" dengan nomor volumenya

    ??? examplecode "Struktur Folder <small>(klik di sini)</small>"
        
        ```
        ├── Manga Folder
        │   ├── _ocr folder
        │   ├── .html
        │   ├── .mokuro
        │   └── .zip
        │        └── file gambar manga (.jpg/.png)
        ```

7. Lanjut ke [Baca Manga yang Sudah Diproses](setup-manga-pc-lazy-guide.md/#baca-manga-yang-sudah-diproses)

---

### Baca Manga yang Sudah Diproses

??? examplecode "Perhatian <small>(klik di sini)</small>"
    Lewati langkah 1 kalau kamu sudah mengikuti [Setup Anki PC](setup-anki-pc-lazy-guide.md)
    

1. Di Anki, tekan ++ctrl+shift+a++ (Windows) atau ++cmd+shift+a++ (MacOS), atau buka `Tools` > `Add-ons`
    - Pilih [AnkiConnect](https://ankiweb.net/shared/info/2055492159), lalu klik `Config`
    - Tambahkan `https://reader.mokuro.app` ke bagian `webCorsOriginList`, atau salin config di bawah ini:

    ??? examplecode "AnkiConnect Config <small>(klik di sini)</small>"

        ```
        {
            "apiKey": null,
            "apiLogPath": null,
            "ignoreOriginList": [],
            "webBindAddress": "127.0.0.1",
            "webBindPort": 8765,
            "webCorsOriginList": [
                "http://localhost",
                "https://killergerbah.github.io",
                "https://reader.mokuro.app",
                "https://app.yatsu.moe",
                "https://app.asbplayer.dev"
                ]
        }
        ```

    ![AnkiConnect PC](img/ankiconnect-pc.png){height=150 width=300}

2. Buka [Mokuro Reader](https://reader.mokuro.app/), klik ikon `Upload` di pojok kanan atas, lalu pilih `choose directory`
    - Pilih folder `Manga` yang berisi manga, file hasil mokuro, dan file `.mokuro`
    - Klik `Upload`

    ![Mokuro upload](img/mokuro-upload.png){height=300 width=600}

3. Di pojok kanan atas, buka `settings` > `Profile` > `Select a File` > [Mokuro Profile](https://drive.google.com/drive/folders/17EzQL9ONQ3MVsCJwC7ejmL0317EwdR--?usp=sharing) > `Import Profiles` > pilih `PC Profile`
    - Kamu juga bisa membuat profil sendiri. Pastikan semua isian di bagian `Anki Connect` sudah diatur
    
     ![Mokuro Settings](img/mokuro-settings.png){height=50 width=100}

4. Untuk mining, cukup tambahkan kata dengan Yomitan seperti biasa
    - Untuk menambahkan screenshot, klik dua kali (atau ketuk dua kali) di dalam `text border`. Bingkai ini tidak terlihat secara bawaan

    ![Mokuro Settings](img/mokuro-yomitan.png){height=400 width=800}

5. Sekarang kamu sudah bisa mining lengkap dengan screenshot dari manga kamu

!!! note "_ocr folder"

    File OCR (folder `_ocr`) tidak wajib disimpan, tapi sebaiknya tetap disimpan

Sekarang kamu sudah bisa mining manga di PC.

<small>Kalau ada masalah, cek [FAQs](setup-manga-pc-lazy-guide.md/#pertanyaan-umum)</small>


---

## Extra Info & Tips

#### Info 1: Shortcut Program OCR

??? info "Shortcut Program OCR <small>(klik di sini)</small>"
    1. Klik kanan di area kosong di desktop, lalu pilih `New` > `Shortcut`

        ![MangaOCR Shortcut](img/mangaocr-shortcut.png){height=300 width=600}

    2. Isi lokasi item seperti ini:
        - Bawaan: `C:\Windows\System32\cmd.exe /k owocr`
        - OCR hanya dari folder tertentu: `C:\Windows\System32\cmd.exe /k owocr -e screenai -j -d -w clipboard -r "\lokasi\ke\folder\screenshot\pilihan"`
            - Contoh: `C:\Windows\System32\cmd.exe /k owocr -e screenai -j -d -w clipboard -r "F:\Pictures\OCR Picture"`
            - Klik `Next`, lalu beri nama shortcut-nya. Selesai.

#### Info 2: Scan pakai Tombol Mouse

??? info "Scan pakai Tombol Mouse <small>(klik di sini)</small>"
    1. Unduh dan pasang [AutoHotkey](https://www.autohotkey.com/)

    2. Unduh [Hotkey](https://drive.google.com/drive/folders/1U94qH4k6L00Wd_96tJBmI2fsOA-HS1uK?usp=sharing) yang sudah disiapkan, lalu jalankan.

    3. Tekan `Forward Button` di mouse untuk menjalankan scan
        - Ini dengan asumsi hotkey `OCR (manga_ocr)` di ShareX masih bawaan, yaitu ++shift+alt+q++
        - Hotkey-nya bisa diubah dengan menyunting script-nya.

---

## Pertanyaan Umum

