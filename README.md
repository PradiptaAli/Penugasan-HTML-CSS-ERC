# GatherUp 2026 — Annual Tech Community Meetup Landing Page

Repositori ini berisi proyek *landing page* interaktif untuk event **GatherUp 2026**, sebuah pertemuan tahunan komunitas teknologi di Yogyakarta. Proyek ini dibangun menggunakan kombinasi HTML5 semantik dan CSS3 modern tanpa menggunakan *framework* eksternal untuk menunjukkan pemahaman dasar rekayasa web yang kuat, rapi, dan responsif.

## 📌 Ikhtisar Proyek
Proyek ini dirancang sebagai platform informasi sekaligus sistem registrasi mandiri (*RSVP*) bagi para calon peserta event. Fokus utama dari desain ini adalah menciptakan antarmuka yang bersih (*clean aesthetics*), tipografi yang memiliki kontras tinggi untuk keterbacaan (*readability*), serta navigasi yang intuitif bagi pengguna.

 Fitur & Implementasi Teknis

1. Struktur Dokumen (HTML5)
* **Semantic Elements:** Menggunakan tag semantik seperti `<nav>`, `<header>`, `<section>`, dan `<footer>` untuk memastikan struktur dokumen yang valid, mudah dipelihara, dan ramah terhadap SEO/aksesibilitas.
* **Asynchronous Embedding:** Integrasi peta lokasi interaktif menggunakan komponen `<iframe>` dari Google Maps yang dikonfigurasi dengan *lazy loading* untuk mengoptimalkan performa pemuatan halaman.
* **Interactive Form Handling:** Menyediakan formulir RSVP fungsional dengan validasi tipe data bawaan (`required`, `type="email"`) untuk menangkap entri nama, email, institusi, dan preferensi sesi acara.
 2. Rekayasa Gaya & Tata Letak (CSS3)
* **Centralized Architecture (CSS Variables):** Manajemen palet warna (*monochrome & off-white accents*), tipe font, dan ukuran radius yang dikelola terpusat menggunakan `:root` variables untuk efisiensi pemeliharaan kode.
* **Modern Layout Engine:**
    * **CSS Grid:** Diimplementasikan pada tata letak kompleks seperti *2x2 statistics unit*, *about section*, dan susunan kartu pembicara (*auto-fit responsive grid*).
    * **Flexbox:** Digunakan untuk komponen linear seperti bilah navigasi (*navbar alignment*), *hero actions*, dan struktur baris bawah pada bagian kaki halaman.
* **Smooth Scrolling System:** Pemanfaatan properti `scroll-behavior: smooth` pada elemen HTML untuk memberikan pengalaman transisi yang halus saat pengguna berinteraksi dengan menu navigasi jangkar (*anchor links*).
* **Fluid Typography:** Menggunakan fungsi `clamp()` pada judul utama (*hero title*) agar ukuran font dapat beradaptasi secara dinamis menyesuaikan lebar *viewport* tanpa mengalami *text-clipping*.
* **Responsive Media Queries:** Pemisahan logika tata letak menggunakan `@media (max-width: 768px)` untuk memastikan fungsionalitas dan estetika halaman tetap prima saat diakses melalui perangkat seluler (mobile-first approach).

📁 Struktur Berkas
```text
├── TEST.html          # Berkas utama dokumen web (Struktur & Konten)
└── style.css          # Berkas stylesheet utama (Desain & Tata Letak)
