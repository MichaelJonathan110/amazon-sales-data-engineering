Amazon Sales Data Engineering
Project Ujian Akhir Semester (UAS) mata kuliah Data Engineering.

Deskripsi
Project ini membangun pipeline ETL (Extract, Transform, Load) dari data penjualan e-commerce Amazon. Data mentah dari Kaggle diekstrak, dibersihkan, dan ditransformasi menggunakan Pentaho Data Integration (Spoon & Carte), lalu hasilnya dimuat ke dalam bentuk tabel bersih untuk dianalisis dan divisualisasikan dengan Power BI.

Tujuan project: menghasilkan dataset penjualan yang konsisten dan siap analisis, serta menyajikan insight penjualan (produk terlaris, tren penjualan, distribusi wilayah) melalui dashboard interaktif.

Arsitektur / Alur Data
Kaggle (Amazon Sale Report.csv) | v [ Extract ] Baca CSV mentah | v [ Transform ] Cleaning, normalisasi, agregasi (Pentaho Spoon) | v [ Load ] Simpan hasil ke tabel bersih (Pentaho Carte) | v [ Visualisasi ] Dashboard interaktif (Power BI)


## Struktur Project

amazon-sales-data-engineering/ |-- data/ | |-- raw/ # Amazon Sale Report.csv (tidak di-commit) | -- processed/ # hasil transformasi (tidak di-commit) |-- etl/ | |-- extract.ktr # transformasi Pentaho: ekstraksi | |-- transform.ktr # transformasi Pentaho: cleaning & agregasi | -- load.ktr # transformasi Pentaho: load |-- dashboard/ | -- amazon_sales.pbix # dashboard Power BI |-- docs/ | -- laporan.pdf # laporan UAS |-- requirements.txt |-- .gitignore `-- README.md

Teknologi yang Digunakan
Pentaho Data Integration (Spoon & Carte) — ETL pipeline
Power BI — visualisasi & dashboard
Microsoft Excel / CSV — sumber & pemeriksaan data
Format data: CSV
Cara Menjalankan
1. Prasyarat
Pentaho Data Integration (Spoon) terpasang
Power BI Desktop terpasang
Java Runtime (untuk Pentaho)
2. Clone repository
git clone https://github.com/USERNAME/amazon-sales-data-engineering.git
cd amazon-sales-data-engineering

### 3. Siapkan data

1. Unduh dataset dari Kaggle: https://www.kaggle.com/datasets/thedevastator/unlock-profits-with-e-commerce-sales-data
2. Letakkan file `Amazon Sale Report.csv` ke folder `data/raw/`

### 4. Jalankan ETL

1. Buka **Spoon** (Pentaho Data Integration)
2. Buka file transformasi di folder `etl/` (`extract.ktr`, `transform.ktr`, `load.ktr`)
3. Jalankan transformasi secara berurutan
4. Hasil bersih akan tersimpan di `data/processed/`

### 5. Buka dashboard

Buka `dashboard/amazon_sales.pbix` dengan **Power BI Desktop**.

## Dataset

- **Sumber:** Kaggle — *Unlock Profits with E-Commerce Sales Data*
- **URL:** https://www.kaggle.com/datasets/thedevastator/unlock-profits-with-e-commerce-sales-data
- **File:** `Amazon Sale Report.csv`
- **Isi:** data transaksi penjualan Amazon (pesanan, produk/SKU, kategori, harga, jumlah, status pengiriman, wilayah, dll.)

> Dataset tidak disertakan di repository (lihat `.gitignore`). Unduh manual dari link di atas dan letakkan di `data/raw/`.

## Hasil / Kesimpulan

- Pipeline ETL berhasil membersihkan dan menstandarkan data penjualan Amazon.
- Dashboard Power BI menampilkan insight seperti produk/kategori terlaris, tren penjualan, dan distribusi pesanan per wilayah.
- Hasil analisis digunakan sebagai dasar rekomendasi bisnis pada laporan UAS.

## Penulis

- **Michael Jonathan Susilo** - 2802449392

## Lisensi

Project ini dibuat untuk keperluan akademik (UAS). Lihat file [LICENSE](LICENSE).


---
