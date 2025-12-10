# 🎁 Interactive LDR / Birthday Digital Gift

Website interaktif berbasis React yang dirancang sebagai hadiah digital spesial (Ulang Tahun / Anniversary / LDR). Proyek ini sepenuhnya **data-driven**, artinya kamu bisa mengubah seluruh teks, foto, musik, dan skenario hanya dengan mengedit satu file JSON tanpa perlu menyentuh kode program (React/JavaScript).

## ✨ Fitur Utama

- **100% Customizable:** Ubah nama, ucapan, dan foto melalui `public/data.json`.
- **LDR Map Animation:** Visualisasi perjalanan paket dari pengirim ke penerima.
- **Interactive Mini-Games:**
  - 🔓 **Slider Lock:** Geser untuk membuka hati.
  - 🔮 **Scratch Card:** Gosok layar untuk melihat pesan rahasia.
  - ❤️ **Heart Pump:** Tap-tap layar untuk mengisi cinta.
- **Cinematic Experience:** Background musik, efek suara, dan kembang api otomatis.
- **Responsive:** Didesain khusus agar tampil cantik di layar HP (Mobile First).

## 📂 Struktur Folder Penting

```text
my-project/
├── public/
│   ├── assets/          <-- TARUH FOTO & MP3 DI SINI
│   ├── data.json        <-- EDIT TEKS & PENGATURAN DI SINI
│   └── index.html
├── src/
│   ├── App.js           <-- Logika Utama (Jangan diubah jika tidak perlu)
│   └── App.css          <-- Styling
└── package.json
```

## 🚀 Cara Menjalankan (Installation)

Pastikan kamu sudah menginstal **Node.js** di komputermu.

1.  **Clone atau Download** repository ini.
2.  Buka terminal di folder proyek.
3.  Install dependencies:
    ```bash
    npm install
    ```
4.  Jalankan server development:
    ```bash
    npm start
    ```
5.  Buka browser di `http://localhost:3000`.

## ⚙️ Cara Kustomisasi (PENTING)

Semua konten diatur di dalam file **`public/data.json`**.

### 1. Mengubah Data Diri & Teks

Buka file `public/data.json`. Struktur datanya dibagi menjadi 3 bagian:

- **`meta`**: Informasi dasar (Nama, Lokasi, Jarak, Umur).
- **`assets`**: Path/lokasi file gambar dan audio.
- **`texts`**: Semua kata-kata yang muncul di layar (Intro, Misi, Surat, dll).

**Contoh Edit `meta`:**

```json
"meta": {
  "targetName": "Nama Target Kamu",
  "senderName": "Nama Kamu",
  "locationSender": "Jakarta",
  "locationTarget": "Surabaya",
  "distance": "780 KM",
  "targetAge": "20"
}
```

### 2. Mengganti Foto & Musik

1.  Siapkan foto-foto kamu (format `.webp`, `.jpg`, atau `.png`) dan musik (`.mp3`).
2.  Masukkan file tersebut ke dalam folder **`public/assets/`**.
3.  Buka `public/data.json` bagian **`assets`** dan sesuaikan nama filenya.

**Contoh Edit `assets`:**

```json
"assets": {
  "photoTarget": "./assets/foto_target.jpg",
  "photoSender": "./assets/foto_aku.jpg",
  "bgm": "./assets/lagu_kesukaan_dia.mp3"
}
```

> **Catatan:** Pastikan nama file di folder dan di JSON **sama persis** (huruf besar/kecil berpengaruh).

### 3. Mengubah Isi Surat

Di bagian `texts` > `letter`, kamu bisa mengubah isi surat. Kamu bisa menambahkan paragraf baru sesuka hati di dalam array `body`.

```json
"letter": {
  "title": "Happy Anniversary!",
  "body": [
    "<strong>Hai Sayang!</strong>",
    "Gak kerasa udah setahun ya kita bareng...",
    "Terima kasih sudah jadi bagian terbaik di hidupku."
  ],
  "closing": "With Love,"
}
```

_Tips: Kamu bisa menggunakan tag HTML seperti `<strong>` untuk menebalkan huruf._

## 🛠️ Tech Stack

- **React JS**: Framework UI.
- **Framer Motion**: Untuk animasi halus dan transisi antar halaman.
- **React Confetti**: Efek kembang api/kertas warna-warni.
- **Canvas API**: Efek kembang api (Fireworks) kustom.

## 🌐 Cara Upload Online (Deploy)

Cara termudah adalah menggunakan **Vercel**:

1.  Push kodingan ini ke GitHub kamu.
2.  Buka [Vercel](https://vercel.com) dan login.
3.  Klik "Add New Project" -> "Import" repository GitHub tadi.
4.  Klik "Deploy".
5.  Selesai! Link website siap dikirim ke doi.

---

Dibuat dengan ❤️ oleh Nabil Aba
