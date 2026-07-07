# Imat Abu Kamal - Portofolio Devfolio

Aplikasi portofolio developer profesional yang modern, elegan, responsif, dan interaktif yang dibangun menggunakan **React**, **Vite**, dan **Tailwind CSS**. 

Aplikasi ini disesuaikan sepenuhnya untuk menampilkan profil, keahlian, riwayat, kontak, serta galeri pencapaian milik **Imat Abu Kamal**.

---

## 🚀 Fitur Utama

1. **Sistem Navigasi Single-Page Tab Dinamis**
   - Berbeda dari navigasi tradisional yang melakukan scrolling panjang, aplikasi ini mengimplementasikan transisi tab eksklusif.
   - Saat Anda meng-klik menu navigasi (Beranda, Tentang, Gallery, Kontak), hanya section yang dipilih yang akan ditampilkan di layar, memberikan pengalaman pengguna yang sangat bersih, cepat, dan terfokus.
   - Menyediakan sinkronisasi tab aktif yang otomatis disesuaikan secara visual pada navbar desktop maupun mobile overlay menu.

2. **Galeri Keahlian Interaktif (Hover Zoom & Rotate)**
   - Galeri keahlian dilengkapi dengan efek hover 3D mikro yang dinamis. 
   - Ikon keahlian akan membesar secara halus (scale-up) dan sedikit berputar (rotate) serta berganti aksen warna dari biru mewah (`#2563eb`) ke ungu gradasi (`#7c3aed`) ketika kursor diarahkan ke kartu keahlian.

3. **Formulir Kontak Dinamis Terintegrasi Google Sheets**
   - Dilengkapi dengan pop-up modal kirim pesan yang interaktif dan aman.
   - Menggunakan integrasi backend via Google Apps Script (tanpa membocorkan API Key di sisi frontend). Data yang dikirim dari formulir kontak langsung divalidasi dan tersimpan di database spreadsheet Google Sheets Anda secara realtime.
   - Sistem validasi input komprehensif di sisi frontend untuk Nama (minimal 2 huruf), Email (format valid), Telepon (dimulai dengan angka '0' & minimal 8 digit), Alamat, dan Pesan.
   - Bar progress animasi pengiriman pesan yang interaktif untuk memberikan feedback instan kepada pengguna saat data sedang dikirim.

4. **Sinkronisasi Dinamis Favicon & Branding**
   - Favicon tab peramban (browser) disinkronkan secara otomatis dan dinamis dengan gambar/foto profil logo yang ada di bagian Navbar, menjaga keselarasan identitas visual merek (branding) Anda.

5. **Responsif Sepenuhnya (Mobile Friendly)**
   - Tampilan dioptimalkan untuk perangkat seluler, tablet, hingga layar desktop ultra-lebar menggunakan teknik fluid grid dan kontainer Tailwind CSS.
   - Dilengkapi dengan navigasi menu hamburger interaktif pada tampilan mobile.

---

## 🛠️ Teknologi yang Digunakan

- **Frontend Framework**: React 19 (TypeScript) & Vite
- **Styling**: Tailwind CSS (Desain modern, bersih, minimalis, dengan palette warna premium Slate & Indigo Blue)
- **Komponen Notifikasi**: SweetAlert2 (Untuk pop-up sukses/gagal kirim pesan yang estetik)
- **Koleksi Ikon**: Font Awesome 6 (Melalui CDN) & Lucide React
- **Tipografi**: Inter (Google Fonts)

---

## 📂 Struktur Proyek Utama

- `index.html`: Entry-point HTML utama yang memuat pustaka CDN Font Awesome, SweetAlert2, serta font kustom.
- `src/main.tsx`: Entry-point aplikasi React.
- `src/App.tsx`: Pusat logika aplikasi, penanganan state tab, validasi form, komunikasi API Google Sheets, serta perenderan markup UI.
- `src/index.css`: File konfigurasi CSS global, animasi kustom untuk Galeri Keahlian, efek popup modal, serta pengaturan scroll.
- `metadata.json`: Metadata platform Google AI Studio untuk konfigurasi identitas aplikasi.

---

## ⚡ Cara Menjalankan secara Lokal

1. Pastikan Anda memiliki **Node.js** terinstal di komputer Anda.
2. Jalankan perintah instalasi dependensi:
   ```bash
   npm install
   ```
3. Jalankan server pengembangan lokal:
   ```bash
   npm run dev
   ```
4. Buka `http://localhost:3000` di browser Anda untuk melihat aplikasi portofolio Anda.
