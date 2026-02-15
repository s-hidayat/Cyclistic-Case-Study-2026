# 🚴 Cyclistic Spatial Analysis: Unlocking Weekend Revenue via Urban Mobility Patterns

![SQL](https://img.shields.io/badge/SQL-DuckDB-yellow?style=for-the-badge&logo=sql)
![R](https://img.shields.io/badge/R-Tidyverse-blue?style=for-the-badge&logo=r)
![Tableau](https://img.shields.io/badge/Viz-Tableau_Geospatial-orange?style=for-the-badge&logo=tableau)
![Status](https://img.shields.io/badge/Status-Completed-green?style=for-the-badge)

> **"Data bukan sekadar angka di spreadsheet; data adalah jejak digital perilaku manusia di ruang kota."**

---

## 👋 Pengantar: Mengapa Proyek Ini Ada?
Sebagai seseorang dengan latar belakang **Arsitektur** yang kini menyelami dunia **Data Analytics**, saya selalu tertarik pada bagaimana manusia berinteraksi dengan lingkungan kota mereka.

Studi kasus **Cyclistic Bike-Share** ini menarik perhatian saya bukan hanya karena volume datanya (5,7 juta baris!), tetapi karena ini adalah masalah **Mobilitas Perkotaan (*Urban Mobility*)**.

Tantangannya sederhana namun krusial: Bagaimana mengubah pengguna sepeda yang hanya bersenang-senang di akhir pekan (*Casual Riders*) menjadi pelanggan setia jangka panjang (*Annual Members*)?

## 🏙️ Pendekatan Unik: The Spatial & Human Angle
Alih-alih hanya membandingkan angka rata-rata, saya mendekati masalah ini dengan kacamata **PropTech**:
* **Mapping Human Flow:** Saya tidak hanya bertanya "kapan" mereka bersepeda, tapi "di mana" mereka berkumpul. Apakah mereka turis pantai atau pekerja kantoran?
* **Space vs. Time:** Menganalisis korelasi antara lokasi stasiun (Taman vs. Gedung Tinggi) dengan durasi penggunaan sepeda.

## 💼 Masalah Bisnis (The Business Case)
Tim pemasaran Cyclistic memiliki data yang jelas:
1.  **Annual Members** adalah sumber pendapatan yang stabil.
2.  **Casual Riders** memberikan profit margin tinggi per transaksi, tapi tidak konsisten.

**Tujuan:** Mengidentifikasi pola perilaku *Casual Riders* yang paling potensial untuk dikonversi menjadi *Members*.

## 🛠️ Tech Stack: Mengapa Excel Tidak Cukup?
Dataset ini berisi **5.719.877 baris data**. Spreadsheet biasa akan *crash*. Oleh karena itu, saya menggunakan pendekatan *Modern Data Stack*:

1.  **SQL (DuckDB via DBeaver):**
    * Digunakan untuk *Heavy Lifting*. Membersihkan data kotor, memfilter anomali (durasi <1 menit), dan mengekstrak metrik waktu.
2.  **R (Tidyverse & ggplot2):**
    * Digunakan untuk analisis statistik mendalam dan validasi hipotesis. R sangat kuat untuk melihat distribusi data yang tidak normal.
3.  **Tableau Public:**
    * Digunakan untuk **Visualisasi Geospasial**. Peta interaktif adalah satu-satunya cara untuk membuktikan hipotesis lokasi (Pantai vs. Kota).

## 📈 Temuan Kunci (Key Insights)

### 1. The "Weekend Warrior" Phenomenon
Data berbicara lantang: Pengguna Casual adalah **"Pejuang Akhir Pekan"**.
* Aktivitas mereka melonjak drastis pada hari **Sabtu & Minggu**.
* Rata-rata durasi bersepeda mereka **2x lebih lama** dibandingkan Member. Ini bukan perjalanan untuk bekerja; ini adalah perjalanan untuk *menikmati hidup*.

### 2. Segregasi Spasial (Pemisahan Lokasi)
Melalui peta panas (*Heatmap*) di Tableau, ditemukan pola yang kontras:
* 🔴 **Casual Riders:** Sangat terkonsentrasi di **garis pantai (*Coastline*)** dan area wisata terbuka seperti Navy Pier.
* 🔵 **Annual Members:** Tersebar merata di **pusat bisnis (*Downtown*)** dan jalur komuter, dengan pola penggunaan jam sibuk (08:00 & 17:00).

### 3. Peluang Musiman (Seasonality)
Musim panas (Juni - Agustus) adalah "Masa Panen". Grafik tren menunjukkan lonjakan masif di bulan-bulan ini, yang berarti kampanye pemasaran harus dimulai sejak bulan Mei (Pre-season).

---

## 💡 Rekomendasi Strategis (Action Plan)
Berdasarkan data, berikut strategi yang saya usulkan:

1.  **📍 Lokasi Adalah Kunci (Geo-Targeting):**
    Berhenti beriklan di pusat kota untuk target Casual. Pasang iklan fisik (QR Code) di stasiun docking sepanjang **jalur pantai dan taman kota**.

2.  **🎟️ Produk Baru: "Summer Weekend Pass":**
    Ciptakan keanggotaan hybrid. Pengguna Casual suka bersepeda lama di akhir pekan musim panas. Berikan mereka paket khusus yang mengakomodasi perilaku ini, sebagai langkah awal masuk ke ekosistem membership.

3.  **gamifikasi Durasi:**
    Karena Casual Riders suka bersepeda lama (>40 menit), buat tantangan *"Mile Hunter"*. Berikan insentif diskon membership jika mereka mencapai jarak tempuh tertentu.

---

## 📊 Lihat Hasil Analisis
Saya percaya visualisasi berbicara lebih keras daripada tabel angka.

* **📄 Baca Analisis Lengkap (Notebook):** [👉 Klik di sini untuk melihat Kode & Narasi di Kaggle](https://www.kaggle.com/samsurhidayat)
* **🗺️ Coba Dashboard Interaktif:** [👉 Klik di sini untuk bermain dengan Peta di Tableau](https://public.tableau.com/views/All_trip_sepeda/Dashboard1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

---

### 📬 Connect with Me
Jika Anda tertarik berdiskusi tentang Data Analytics, PropTech, atau Arsitektur:

* **LinkedIn:** [Nama LinkedIn Anda]
* **Portfolio:** [Link Portfolio/GitHub Anda]

---
*Analisis ini dibuat sebagai bagian dari Google Data Analytics Professional Certificate.*
