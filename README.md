# Surya Mataram

![Status](https://img.shields.io/badge/Status-Active-10b981?style=for-the-badge)
![Developer](https://img.shields.io/badge/Developer-fatur62-d4af37?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)
![Tech](https://img.shields.io/badge/Tech-HTML5%20%7C%20CSS3%20%7C%20ES6%2B-08090c?style=for-the-badge)

**Surya Mataram** adalah aplikasi web *single-page* yang memadukan perhitungan astronomi **Jam Matahari Hakiki (*True Solar Time*)** dengan tiga sistem penanggalan peradaban (**Gregorian**, **Hijriyah**, dan **Kalender Jawa Sultan Agungan**) serta kalender ekologi-agraris **Pranata Mangsa**. Dirancang dengan estetika *Royal Javanese Gold & Obsidian Glassmorphism*.

---

## Fitur Utama

### 1. Penunjuk Waktu Ganda (Dual Astronomical & Civil Clocks)
* **Waktu Jam Matahari (*True/Apparent Solar Time*):** Menghitung waktu surya sejati secara *real-time* menggunakan persamaan waktu astronomis (*Equation of Time* / rumus Spencer) serta koreksi garis bujur (*Longitude Meridian Correction*).
* **Waktu Jam Standar Umum (*Civil Time*):** Menampilkan waktu zona standar lokal (WIB/UTC) secara akurat beserta indikator selisih menit terhadap posisi matahari.
* **Multi-Meridian & Geolocation GPS:** Mendukung pemilihan titik meridian kota-kota penting (Yogyakarta, Surakarta, Jakarta, Surabaya, Makkah) maupun deteksi koordinat GPS pengguna secara otomatis.

### 2. Tiga Sistem Kalender Terintegrasi
* **Sistem Internasional (Gregorian):** Menampilkan tanggal masehi, hari ke- dalam setahun (*Day of Year*), pekan ISO, status tahun kabisat/basitah, dan *Julian Day Number* (JDN).
* **Sistem Kamariyah (Hijriyah):** Berbasis hisab *Umm al-Qura* dengan *fallback* algoritma Kuwaiti/Tabular, dilengkapi nama hari bahasa Arab dan estimasi fase bulan (*Moon Phase*).
* **Sistem Nusantara (Sultan Agungan):**
  * Menampilkan kombinasi **Saptawara** (7 hari) dan **Pancawara / Pasaran** (*Legi, Pahing, Pon, Wage, Kliwon*) lengkap dengan bahasa Krama.
  * Kalkulasi otomatis **Total Neptu** (Dina + Pasaran).
  * Perhitungan siklus **Wuku** (30 Wuku / 210 hari), **Tahun Jawa** (*Alip, Ehe, Jimawal, Je, Dal, Be, Wawu, Jimakir*), dan **Windu** (*Adi, Kuntara, Sengara, Sancaya*) sesuai Kurup Asapon.

### 3. Kalender Ekologi Jawa: Pranata Mangsa
* Memetakan tanggal masehi ke dalam 12 musim **Pranata Mangsa** (*Kasa* hingga *Saddha*).
* Menyajikan informasi **Candraning Mangsa** (simbol alam), kondisi ekologi, panduan aktivitas pertanian, durasi hari (termasuk penyesuaian tahun kabisat pada *Mangsa Kawolu*), dan indikator persentase perjalanan mangsa.

---

## Arsitektur Teknis

* **Zero Dependencies:** Murni dibangun dengan HTML5 Semantik, CSS3 (Flexbox, Grid, Custom Properties), dan Vanilla JavaScript (ES6+) tanpa *framework* tambahan.
* **Safe JSON Data Handling:** Seluruh struktur data kalender dikelola dalam format JSON terpusat yang divalidasi secara ketat menggunakan blok `try-catch` dan pengecekan *null/undefined*.
* **Simulasi Lintas Tanggal:** Tersedia fitur *Date Picker* untuk meninjau konversi weton, hijriyah, dan pranata mangsa pada tanggal berapa pun di masa lalu maupun masa depan.

---

## Cara Penggunaan

1. *Clone* repositori ini ke komputer Anda:
   ```bash
   git clone [https://github.com/fatur62/surya-mataram.git](https://github.com/fatur62/surya-mataram.git)
