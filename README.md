
#  Cyclistic Case Study: Strategi Konversi Pengendara Berbasis Data

![SQL](https://img.shields.io/badge/SQL-DuckDB-yellow?style=for-the-badge&logo=sql)
![R](https://img.shields.io/badge/R-Tidyverse-blue?style=for-the-badge&logo=r)
![Tableau](https://img.shields.io/badge/Viz-Tableau_Geospatial-orange?style=for-the-badge&logo=tableau)
![Status](https://img.shields.io/badge/Status-Completed-green?style=for-the-badge)

## 📌 Ringkasan Proyek
Proyek ini bertujuan untuk memecahkan masalah pemasaran utama Cyclistic: **Bagaimana cara mengonversi Pengendara Kasual (*Casual Riders*) menjadi Anggota Tahunan (*Annual Members*)?**

Menganalisis lebih dari **5,7 juta data perjalanan** sepanjang tahun 2025, studi ini mengungkap perbedaan perilaku fundamental antara kedua tipe pengguna—mulai dari *kapan* mereka berkendara, *berapa lama* durasinya, hingga *di mana* lokasi favorit mereka.

## 🛠️ Metodologi & Tech Stack
Karena volume data mencapai 5,7 juta baris, spreadsheet konvensional tidak lagi efisien. Saya menggunakan pendekatan *Modern Data Stack* berikut:

1.  **SQL (DuckDB via DBeaver):**
    * Digunakan untuk *Data Cleaning* dan pemrosesan awal.
    * Memfilter anomali data (durasi < 1 menit atau > 24 jam).
    * Memastikan presisi data lokasi (Latitude/Longitude) untuk pemetaan.
2.  **R (Tidyverse):**
    * Digunakan untuk analisis statistik mendalam dan visualisasi grafik statis.
    * Memverifikasi logika pembersihan data.
3.  **Tableau Public:**
    * Digunakan untuk visualisasi Geospasial (Peta Sebaran) dan Analisis Temporal (Heatmap).

## 📈 Temuan Kunci (Key Insights)

Berdasarkan analisis data, ditemukan pola perilaku yang sangat kontras:

### 1. Komposisi Pengguna (Market Share)
Meskipun **Annual Members mendominasi 65%** dari total perjalanan, segmen **Casual Riders (35%)** merupakan pasar potensial yang cukup besar untuk dikonversi.

### 2. Durasi Berkendara (Duration)
Pengendara Kasual menghabiskan waktu rata-rata **2x lebih lama** bersepeda dibandingkan Anggota Tahunan. Ini mengindikasikan bahwa Casual Riders menggunakan sepeda untuk tujuan santai/rekreasi, bukan sekadar transportasi cepat.

### 3. Pola Mingguan (The "Weekend Warrior")
* **Casual Riders:** Aktivitas melonjak drastis pada akhir pekan (**Sabtu & Minggu**).
* **Annual Members:** Mendominasi penggunaan pada hari kerja (Senin-Jumat), memperkuat dugaan penggunaan untuk komuter kerja.

### 4. Segregasi Lokasi & Waktu (Map & Heatmap)
* **Lokasi:** Peta panas (*Heatmap*) menunjukkan Pengendara Kasual terkonsentrasi di area **wisata dan pesisir pantai**. Sebaliknya, Member tersebar di pusat bisnis.
* **Musiman:** Lonjakan tertinggi terjadi pada **Musim Panas (Juni - Agustus)**.

## 💡 Rekomendasi Bisnis (Action Plan)
Berdasarkan bukti data di atas, berikut adalah strategi yang direkomendasikan:

1.  **Strategi Lokasi (Coastal Dominance):**
    Prioritaskan pemasangan iklan fisik (Billboards/QR Code) di stasiun docking sepanjang **jalur pantai**. Gunakan pesan kampanye bernuansa *"Liburan Tanpa Batas"* untuk memikat segmen rekreasi ini.

2.  **Produk Baru ("Summer Weekend Pass"):**
    Karena Casual Riders aktif di akhir pekan musim panas, luncurkan paket keanggotaan khusus (misal: *Weekend-Only Membership*). Ini memberikan opsi yang lebih relevan bagi mereka dibanding keanggotaan penuh tahunan.

3.  **Gamifikasi Durasi:**
    Manfaatkan kebiasaan durasi panjang Casual Riders. Buat tantangan di aplikasi (misal: *"Gowes 10 Jam Bulan Ini"*) dengan hadiah diskon *upgrade* ke Annual Member bagi mereka yang mencapainya.

---

## 🔗 Lihat Analisis Lengkap

* **📄 Notebook (Kode & Narasi):** [Lihat di Kaggle](https://www.kaggle.com/samsurhidayat)
* **🗺️ Dashboard Interaktif:** [Lihat di Tableau Public](https://public.tableau.com/views/All_trip_sepeda/Dashboard1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

---
* **LinkedIn:** [Samsur Hidayat](https://www.linkedin.com/in/s-hidayat-69b1b5372)

*Analisis ini dibuat sebagai bagian dari Google Data Analytics Professional Certificate.*
