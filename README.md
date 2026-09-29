## **PRODUCT REQUIREMENTS DOCUMENT (PRD) SMA N 1 Rembang**
---
## **1. Informasi Produk**

| Item                | Detail                                                                             |
| ------------------- | ---------------------------------------------------------------------------------- |
| **Nama Produk**     | Website Profil Sekolah SMA N 1 Rembang                                                 |
| **Jenis Produk**    | Website Informasi & Profil Institusi                                               |
| **Target Pengguna** | Siswa, calon siswa, orang tua, guru, alumni, masyarakat                            |
| **Platform**        | Web Responsive                                                                     |
| **Tujuan**          | Menyediakan informasi resmi sekolah secara terstruktur, menarik, dan mudah diakses |

---

## **2. Latar Belakang**

Website ini dibuat sebagai media informasi digital untuk memperkenalkan SMA Negeri 1 Rembang kepada pengunjung.

Informasi yang disediakan mencakup sambutan kepala sekolah, visi dan misi sekolah, program peminatan yang tersedia, jumlah siswa berdasarkan jurusan, serta informasi kontak sekolah.

Website dirancang dengan navigasi sederhana agar pengunjung dapat mengakses informasi utama melalui tiga halaman, yaitu Home, Jurusan, dan Kontak.

---

## **3. Tujuan Produk**

* Menyediakan informasi dasar mengenai SMA Negeri 1 Rembang.
* Menampilkan sambutan dari kepala sekolah.
* Menyampaikan visi dan misi sekolah.
* Menampilkan informasi program peminatan yang tersedia.
* Menampilkan jumlah siswa pada masing-masing program peminatan.
* Menyediakan informasi kontak sekolah.
* Menyediakan formulir untuk mengirimkan pesan.
---

## **4. Target Pengguna**

### Pengunjung Umum

Pengunjung dapat memperoleh informasi umum mengenai sekolah, visi dan misi, program peminatan, serta informasi kontak.

### Siswa dan Calon Siswa

Pengguna dapat melihat informasi mengenai program peminatan yang tersedia beserta deskripsi dan jumlah siswa pada setiap jurusan.

### Orang Tua

Pengguna dapat memperoleh informasi dasar mengenai sekolah serta informasi kontak yang dapat digunakan untuk menghubungi sekolah.

### Guru / Staff

Website dapat menjadi media untuk menyampaikan informasi dasar mengenai identitas dan program sekolah.

---

## **5. Struktur Website**

Website memiliki tiga halaman utama:

```
Website Profil SMA Negeri 1 Rembang
│
├── Home
│   ├── Hero / Welcome
│   ├── Sambutan Kepala Sekolah
│   └── Visi & Misi
│
├── Jurusan
│   ├── Program Peminatan
│   │   ├── IPA
│   │   ├── IPS
│   │   └── Bahasa
│   │
│   └── Jumlah Siswa per Jurusan
│
└── Kontak
    ├── Formulir Kontak
    └── Informasi Kontak
```
---

## **6. Functional Requirements**

### FR-01 — Navigasi

Halaman beranda memiliki:

Website menyediakan navigasi utama yang terdiri dari:

* Home
* Jurusan
* Kontak
  
Navigasi tersedia pada seluruh halaman sehingga pengguna dapat berpindah antarhalaman. Halaman yang sedang aktif ditandai melalui aria-current="page" dan styling navigasi.

---

### FR-02 — Halaman Home

Halaman Home berfungsi sebagai halaman utama website.

**Hero Section**

Hero section menampilkan:

* Nama sekolah
* Judul sambutan
* Deskripsi singkat website
* Foto latar sekolah

Teks utama yang ditampilkan:

> Selamat Datang di SMA Negeri 1 Rembang

Hero juga menjelaskan bahwa website menyediakan informasi mengenai sekolah, program peminatan, dan cara menghubungi sekolah.

**Sambutan Kepala Sekolah**

Bagian sambutan menampilkan:

* Foto kepala sekolah
* Sambutan kepala sekolah
* Nama kepala sekolah
* Jabatan kepala sekolah

Kepala sekolah yang ditampilkan adalah:

**Endang Sri Lestari, S.Pd.**
**Kepala SMA Negeri 1 Rembang**

Bagian visi dan misi menampilkan:

**Visi:**

> "Berjatidiri dan Maju dalam Prestasi"

**Misi:**

1. Mewujudkan lembaga pendidikan yang bernuansa keagamaan, kebangsaan, keilmuan, dan wawasan lingkungan.
2. Mewujudkan lembaga pendidikan yang memiliki daya saing sampai di tingkat internasional.
---

### FR-03 — Halaman Jurusan

Halaman Jurusan menyediakan informasi mengenai program peminatan yang tersedia di SMA Negeri 1 Rembang.

Website menampilkan tiga program peminatan:

**1. IPA — Ilmu Pengetahuan Alam**

Membekali siswa dengan pemahaman mendalam dalam bidang sains dan matematika melalui pembelajaran yang logis, analitis, dan berbasis pemecahan masalah.

**2. IPS — Ilmu Pengetahuan Sosial**

Membekali siswa dengan wawasan mengenai ilmu sosial, ekonomi, geografi, dan sejarah untuk memahami berbagai fenomena dalam kehidupan masyarakat.

**3. Bahasa**

Mengembangkan kemampuan siswa dalam berbahasa, bersastra, dan berkomunikasi secara efektif serta memperluas wawasan terhadap keberagaman budaya.

#### Data Jumlah Siswa

Website menyediakan tabel jumlah siswa berdasarkan program peminatan untuk Tahun Ajaran 2026:

| Jurusan   |  Jumlah Siswa |
| --------- | ------------: |
| IPA       |     180 siswa |
| IPS       |     120 siswa |
| Bahasa    |      60 siswa |
| **Total** | **360 siswa** |

---

## FR-04 — Halaman Kontak

Halaman Kontak menyediakan dua bagian utama:

1. Formulir kontak
2. Informasi kontak sekolah

**Formulir Kontak**

Formulir menyediakan input:

* Nama
* Email
* Pesan
* Tombol Kirim Pesan

Field nama, email, dan pesan ditetapkan sebagai field yang wajib diisi menggunakan atribut `required`.

> **Catatan implementasi:** formulir saat ini belum terhubung dengan backend atau sistem penyimpanan pesan. Form menggunakan `action="#"` dan `method="post"`, sehingga PRD ini tidak mengklaim bahwa pesan sudah benar-benar dikirim atau disimpan.

**Informasi Kontak**

Website menampilkan:

* **Alamat:** Jalan Gajah Mada No. 5, Desa Magersari, Kecamatan Rembang, Kabupaten Rembang, Provinsi Jawa Tengah
* **Telepon:** (0295) 691375
* **Email:** [sma1rbg@yahoo.co.id](mailto:sma1rbg@yahoo.co.id)
* **Jam Layanan:** Senin – Jumat, 07.00 – 15.00 WIB


---

## **7. Admin / Content Management**

Belum tersedia untuk versi saat ini.

---

## **8. User Flow**

#### Pengunjung Umum

```text
                Website
                   │
                   ▼
                Home
             ┌─────┼─────┐
             │     │     │
             ▼     ▼     ▼
           Home  Jurusan Kontak
                   │       │
                   ▼       ▼
              Info       Form &
             Jurusan    Informasi
```

#### User Flow Calon Siswa

```text
Home
 │
 ├── Melihat informasi sekolah
 │
 ├── Membaca sambutan kepala sekolah
 │
 ├── Melihat visi & misi
 │
 ▼
Jurusan
 │
 ├── Melihat IPA
 ├── Melihat IPS
 └── Melihat Bahasa
 │
 ▼
Melihat jumlah siswa
 │
 ▼
Kontak
 │
 ├── Melihat informasi kontak
 └── Mengisi formulir pesan
```

---

## **9. Non-Functional Requirements**

### 9.1 Responsive Design

Website harus dapat menyesuaikan tampilan dengan ukuran layar yang berbeda.

Pada ukuran layar lebih kecil:

* Navigasi menyesuaikan jarak antar-item.
* Section sambutan berubah menjadi satu kolom.
* Section visi & misi berubah menjadi satu kolom.
* Section kontak berubah menjadi satu kolom.
* Daftar jurusan berubah menjadi satu kolom.
* Footer berubah menjadi layout vertikal.

### 9.2 Accessibility

Website menggunakan:

* `alt` text pada gambar.
* Semantic HTML seperti `header`, `nav`, `main`, `section`, `footer`, `form`, dan `table`.
* `aria-current="page"` untuk menunjukkan halaman aktif.
* Label pada setiap field formulir.
* `scope="col"` pada header tabel.

### 9.3 Visual Design

Website menggunakan:

* Warna utama navy blue.
* Warna aksen gold.
* Background putih dan light blue.
* Font **Poppins** untuk heading.
* Font **Inter** untuk body text.
* Layout berbasis container dengan maximum width 1140px.

---

## **10. Teknologi**

Teknologi yang digunakan dalam implementasi:

| Teknologi        | Penggunaan                         |
| ---------------- | ---------------------------------- |
| **HTML5**        | Struktur halaman dan konten        |
| **CSS3**         | Styling, layout, responsive design |
| **Google Fonts** | Font Poppins dan Inter             |
| **Git & GitHub** | Version control dan repository     |
| **Vercel**       | Deployment website                 |

Source HTML menggunakan HTML5 dengan struktur semantic HTML dan menghubungkan setiap halaman ke satu stylesheet `style.css`.

---

## **11. Prioritas Fitur**

#### MVP / Current Implementation

* Beranda
* Jurusan
* Kontak
* Responsive design
* Navigation

#### Pengembangan Berikutnya

* Backend formulir kontak
* Database
* Admin dashboard
* CMS
* Berita
* Galeri
* PPDB
* Google Maps
* dll.

## **12. Struktur Project**

Struktur project berdasarkan file yang digunakan:

```text
Pweb-Assignment/Week 3
│
├── index.html
├── jurusan.html
├── kontak.html
├── style.css
│
└── assets/
    ├── logo.png
    ├── hero.jpg
    └── kepala-sekolah.png
```

> Struktur `assets/` disesuaikan dengan referensi file gambar yang digunakan oleh HTML dan CSS.

---
