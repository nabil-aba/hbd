# 🎉 Koleksi Template Ucapan Selamat Ulang Tahun Interaktif

Selamat datang! Repositori ini adalah kumpulan template halaman web ucapan selamat ulang tahun yang modern, interaktif, dan mudah dikustomisasi. Setiap folder di sini adalah sebuah proyek mandiri yang bisa kamu ambil, personalisasi, dan kirimkan kepada orang tersayang.

Tujuan proyek ini adalah menyediakan cara yang unik dan berkesan untuk merayakan hari spesial seseorang, tanpa perlu melakukan coding dari nol.

---

## Fitur Utama

*   **🎨 Mudah Dikustomisasi:** Cukup ubah satu file `data.json` untuk mengganti nama, pesan, tanggal, dan foto.
*   **✨ Animasi Menarik:** Dilengkapi dengan animasi halus untuk memberikan efek "wow".
*   **📱 Responsif:** Tampil sempurna di berbagai perangkat, mulai dari ponsel hingga desktop.
*   **🚀 Siap Pakai:** Tidak perlu proses _build_. Ambil foldernya, edit datanya, dan langsung hosting.

---

## Cara Membuat Versi Kamu Sendiri

Kamu tidak perlu meng-clone seluruh repositori ini. Cukup ambil satu folder template yang kamu suka. Berikut adalah cara termudah untuk melakukannya.

### Metode 1: `degit` (Cara Paling Cepat & Direkomendasikan)

Ini adalah cara terbaik jika kamu hanya ingin salinan bersih dari template tanpa history Git. Pastikan kamu sudah menginstall [Node.js](https://nodejs.org/).

1.  Buka terminal atau Command Prompt.
2.  Jalankan perintah di bawah ini. Perintah ini akan membuat folder baru (`ucapan-untuk-budi`) yang berisi salinan template (`theme-1`).

    ```bash
    # Format: npx degit <user>/<repo>/<folder_template> <nama_folder_barumu>
    npx degit nabil-aba/hbd-public/theme-1 ucapan-untuk-budi
    ```

3.  Masuk ke folder baru tersebut.

    ```bash
    cd ucapan-untuk-budi
    ```

**Selesai!** Sekarang kamu sudah memiliki semua file yang dibutuhkan dan siap untuk kustomisasi.

---

### Metode 2: Git Sparse Checkout (Untuk Pengguna Mahir)

Gunakan cara ini jika kamu ingin tetap terhubung dengan repositori ini untuk mendapatkan pembaruan template di masa depan.

1.  **Clone repositori tanpa mengunduh file:**
    ```bash
    git clone --filter=blob:none --no-checkout https://github.com/nabil-aba/hbd-public.git
    cd hbd-public
    ```

2.  **Aktifkan sparse checkout dan pilih template:**
    ```bash
    git sparse-checkout init --cone
    git sparse-checkout set theme-1 # Ganti 'theme-1' dengan nama template lain
    ```

3.  **Salin folder template ke luar untuk dijadikan proyek baru:**
    ```bash
    # Keluar dari direktori
    cd ..
    # Salin folder menjadi proyek baru
    cp -r hbd-public/theme-1 ucapan-untuk-budi
    ```

---

Kamu perlu meng-hostingnya agar bisa diakses melalui link. Berikut beberapa platform gratis yang sangat mudah digunakan:

*   **Netlify Drop:** Cukup buka [Netlify Drop](https://app.netlify.com/drop) dan seret (drag and drop) folder proyekmu (`ucapan-untuk-budi`) ke dalam browser. Dalam beberapa detik, kamu akan mendapatkan link yang bisa dibagikan.
*   **Vercel:** Mirip seperti Netlify, sangat mudah untuk men-deploy situs statis.
*   **GitHub Pages:** Jika kamu ingin menjadikan proyek ini repositori Git-mu sendiri, kamu bisa mengaktifkan GitHub Pages untuk mendapatkan hosting gratis.

Cukup bagikan link yang kamu dapatkan, dan berikan kejutan terbaik di hari ulang tahun mereka!
