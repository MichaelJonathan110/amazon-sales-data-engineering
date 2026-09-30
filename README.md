# UAS Data Engineering
> Project Ujian Akhir Semester (UAS) mata kuliah Data Engineering.
## Deskripsi
Tuliskan 2-4 kalimat: latar belakang, masalah, dan hasil/insight utama.
## Arsitektur / Alur Data
Sumber Data -> Ingestion -> Transformasi (ETL) -> Penyimpanan -> Visualisasi/Output
## Struktur Project
- data/         : data mentah & hasil olahan (tidak di-commit)
- notebooks/    : Jupyter notebook eksplorasi & analisis
- src/          : kode sumber / script pipeline
- outputs/      : hasil (grafik, laporan) (tidak di-commit)
- requirements.txt
- .gitignore
- README.md
## Teknologi
- Python 3.x
- pandas, numpy, matplotlib (sesuaikan)
- Lainnya: (mis. PostgreSQL, Airflow, Docker)
## Cara Menjalankan
1. Prasyarat: python --version  (min 3.10)
2. Clone: git clone https://github.com/USERNAME/NAMA-REPO.git
3. Env: python -m venv .venv  lalu  .venv\Scripts\activate  lalu  pip install -r requirements.txt
4. Jalankan: python src/main.py  (atau jupyter notebook)
## Dataset
Jelaskan sumber data, ukuran, dan cara memperolehnya. Jangan commit data besar/sensitif.
## Hasil / Kesimpulan
Ringkas temuan atau output penting.
## Penulis
- Nama Anda - NIM - Kelas
## Lisensi
MIT - lihat file LICENSE.
