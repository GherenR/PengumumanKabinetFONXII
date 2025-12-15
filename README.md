# Pengumuman Kabinet FON XII 🇮🇩

Website resmi untuk pengumuman dan informasi terkait **Kabinet Forum OSIS Nasional (FON) Angkatan XII**. Proyek ini bertujuan untuk memberikan informasi yang mudah diakses mengenai struktur kabinet, visi-misi, dan pengumuman terbaru bagi seluruh pengurus dan anggota.

## 📸 Tampilan (Screenshots)
![Tampilan Website](https://i.ibb.co.com/pvQ39GKm/Preview-Porto1.png)

## 🚀 Fitur Utama
* **Responsive Design:** Tampilan menyesuaikan perangkat (Desktop & Mobile).
* **Pengumuman:** Halaman khusus untuk update berita terbaru organisasi.

## 🛠️ Teknologi yang Digunakan
Proyek ini dibangun menggunakan teknologi web dasar:
* **HTML5 (HyperText Markup Language):** Digunakan sebagai kerangka utama struktur halaman web (DOM), termasuk penyusunan header, content, dan footer.
* **CSS3 (Cascading Style Sheets):** Digunakan untuk mempercantik tampilan (styling) dan mengatur tata letak (layout) agar responsif di berbagai perangkat (Desktop & Mobile).
* **JavaScript (Vanilla JS):** Digunakan untuk memberikan interaktivitas pada halaman, seperti animasi scrolling, menu navigasi responsif (hamburger menu), dan logika tampilan dinamis.
* **Version Control System (Git & GitHub):** Digunakan untuk manajemen kode sumber dan deployment melalui GitHub Pages.
* **Code Editor:** Visual Studio Code.

## 💻 Cara Menjalankan (Local)
Karena website ini bersifat statis (*static site*), Anda tidak perlu menginstal *dependencies* apapun.

1.  **Clone** repositori ini:
    ```bash
    git clone [https://github.com/GherenR/PengumumanKabinetFONXII.git](https://github.com/GherenR/PengumumanKabinetFONXII.git)
    ```
2.  Buka folder proyek.
3.  Klik dua kali file `index.html` untuk membukanya di browser (Chrome, Firefox, Edge, dll).

## 🌐 Cara Publish (Deploy) ke Website
Proyek ini dapat diubah menjadi website aktif yang bisa diakses publik secara **gratis** menggunakan fitur **GitHub Pages**.

Jika Anda ingin men-deploy proyek ini (menjadikannya website online), ikuti langkah berikut:

1.  Masuk ke tab **Settings** di repository ini.
2.  Di menu sebelah kiri, cari dan klik bagian **Pages**.
3.  Pada bagian **Build and deployment**, pastikan Source diatur ke **Deploy from a branch**.
4.  Di bagian **Branch**, pilih `main` dan folder `/ (root)`.
5.  Klik tombol **Save**.
6.  Tunggu sejenak, link website akan muncul (contoh: `https://gherenr.github.io/PengumumanKabinetFONXII`).

## Penjelasan Alur Logika: Sistem bekerja dengan model Client-Side Rendering. Ketika pengguna mengakses URL:

1. Browser akan memuat file index.html sebagai kerangka.
2. Browser secara paralel memuat file styles.css untuk menerapkan desain visual.
3. Browser memuat aset gambar dari folder images/.
4. Terakhir, browser mengeksekusi app.js untuk mengaktifkan fungsi interaktif (tombol/navigasi).
5. Halaman siap digunakan oleh pengguna.

## ⚙️ Kustomisasi & Cara Edit
Website ini dirancang sebagai *template* yang mudah disesuaikan untuk kebutuhan organisasi Anda. Anda dapat mengubah elemen visual dan konten tanpa harus mengubah struktur kode yang rumit.

Berikut adalah panduan untuk mengubah elemen utama:

### 1. Mengubah Gambar & Logo 🖼️
Semua aset gambar tersimpan di folder `images/`.
* **Logo Organisasi:** Ganti file logo lama dengan logo organisasi Anda. Pastikan nama filenya disesuaikan di `index.html` (bagian tag `<img>`).
* **Background:** Untuk mengganti latar belakang, cukup timpa file gambar background yang ada di folder `images/` atau ubah link gambarnya di file `styles.css` / `index.html`.

### 2. Mengubah Teks & Pengumuman 📝
Seluruh konten teks dapat diedit langsung melalui file `index.html`.
* **Judul & Nama Kabinet:** Cari teks nama kabinet di bagian `<header>` atau `<h1>` dan ubah sesuai nama organisasi Anda.
* **Isi Pengumuman:** Anda bisa mengedit paragraf deskripsi untuk menyesuaikan pesan yang ingin disampaikan.

### 3. Mengatur Waktu/Tanggal 📅
Untuk mengubah tanggal pengumuman atau *countdown* (jika ada):
* Buka file `app.js`.
* Cari bagian variabel teks "duedate".
* Ganti dengan tanggal dan waktu spesik target yang Anda inginkan.

---

## 📂 Struktur Folder
```text
/
├── images/       # Aset gambar untuk website
├── app.js        # Logika JavaScript
├── index.html    # Halaman utama
├── styles.css    # File styling CSS
└── README.md     # Dokumentasi proyek
