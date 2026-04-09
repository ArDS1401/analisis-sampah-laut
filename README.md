# [cite_start]Analisis Pengaruh Sampah Laut terhadap Populasi Makhluk Hidup Laut [cite: 15]

## [cite_start]1. Executive Summary [cite: 14]

[cite_start]**Project Overview** [cite: 16]
* [cite_start]**Tujuan Project**: Penelitian ini bertujuan untuk menganalisis pengaruh sampah laut terhadap populasi makhluk hidup laut dengan mengidentifikasi hubungan antara tingkat pencemaran sampah dan perubahan jumlah populasi organisme laut dari waktu ke waktu. [cite: 17] 
* [cite_start]**Fokus Penelitian**: Penelitian ini juga bertujuan untuk mengetahui jenis sampah yang paling dominan serta spesies yang paling terdampak oleh pencemaran tersebut. [cite: 18] [cite_start]Melalui pendekatan analisis data dan visualisasi statistik, diharapkan penelitian ini dapat memberikan gambaran mengenai sejauh mana sampah laut memengaruhi keseimbangan ekosistem laut serta menjadi dasar dalam upaya pengelolaan dan pengendalian pencemaran lingkungan laut. [cite: 19]
* [cite_start]**Scope Project**: Ruang lingkup project ini mencakup integrasi data jumlah sampah laut, khususnya sampah plastik dan mikroplastik, dengan data populasi makhluk hidup laut pada periode waktu tertentu. [cite: 20] [cite_start]Data yang digunakan meliputi volume atau tingkat pencemaran sampah laut, jumlah populasi spesies laut, serta informasi wilayah perairan yang dianalisis. [cite: 21] [cite_start]Project ini berfokus pada analisis hubungan antara tingkat pencemaran dan perubahan populasi menggunakan metode statistik dan visualisasi data, tanpa melakukan pengambilan data lapangan secara langsung. [cite: 22]
* [cite_start]**Timeline**: 3 Bulan (Februari - Mei) [cite: 30]

[cite_start]**Expected Outcomes**: [cite: 23]
* [cite_start]Insight mengenai hubungan antara tingkat sampah laut dan perubahan populasi makhluk hidup laut [cite: 24]
* [cite_start]Identifikasi spesies yang paling terdampak pencemaran [cite: 25]
* [cite_start]Visualisasi tren pencemaran dan penurunan populasi per wilayah/periode waktu [cite: 26]
* [cite_start]Model Machine Learning untuk memprediksi dampak peningkatan sampah plastik terhadap populasi biota laut [cite: 27]
* [cite_start]Klasifikasi wilayah pesisir berdasarkan tingkat risiko ekologis [cite: 28]
* [cite_start]Rekomendasi berbasis data untuk pengelolaan dan pengurangan sampah laut [cite: 29]

---

## [cite_start]2. Stakeholders [cite: 31]

* [cite_start]**Project Owner**: Kementerian Kelautan dan Perikanan (KKP) [cite: 32]
* [cite_start]**End Users**: [cite: 39]
    * [cite_start]Pemerintah Daerah (wilayah pesisir) [cite: 40]
    * [cite_start]Kementerian Kelautan dan Perikanan [cite: 42]
    * [cite_start]Dinas Lingkungan Hidup [cite: 43]

### [cite_start]Team Members [cite: 33]

| Nama | NIM | Role |
| :--- | :--- | :--- |
| [cite_start]**Arie Dwi Sulistyo** [cite: 9] | (244311004) [cite_start][cite: 9] | [cite_start]Project Manager [cite: 34] |
| [cite_start]**Muhammad Rofiqul A.** [cite: 9] | (244311019) [cite_start][cite: 9] | [cite_start]Data Engineer [cite: 36] |
| [cite_start]**Dila Alif Regita** [cite: 9] | (244311010) [cite_start][cite: 9] | [cite_start]Data Analyst [cite: 38] |
| [cite_start]**Suqya Rohmatin** [cite: 9] | (244311028) [cite_start][cite: 9] | [cite_start]Data Analyst [cite: 38] |

> [cite_start]**Dosen Pengampu**: Gus Nanang Syaifuddiin, S.Kom., M.Kom. [cite: 10]
> [cite_start]**Program Studi**: TRPL, JURUSAN TEKNIK [cite: 11, 12]
> [cite_start]**Institusi**: POLITEKNIK NEGERI MADIUN 2026 [cite: 13]

---

## [cite_start]3. Data Source Analysis [cite: 44]

### [cite_start]3.1 Data Pemerintah (data.go.id) [cite: 45]
* [cite_start]**Dataset Name**: Timbulan Sampah dan Komposisi Sampah (Fokus Wilayah Pesisir/Kabupaten) [cite: 47]
* [cite_start]**Data Owner**: Kementerian Lingkungan Hidup dan Kehutanan (KLHK) [cite: 50]
* [cite_start]**URL/Access Point**: https://sipsn.menlhk.go.id/sipsn/ & https://data.go.id/ [cite: 48, 49]
* [cite_start]**Update Frequency**: Semesteran / Tahunan [cite: 51]
* [cite_start]**Time Coverage**: 2015 - 2024 [cite: 55]
* [cite_start]**Format Data**: CSV, Excel, Web Dashboard [cite: 53]
* [cite_start]**Data Quality**: [cite: 56]
    * **Completeness**: Medium (~70-80%). Bergantung pada kepatuhan pelaporan masing-masing pemerintah daerah. [cite_start]Beberapa kabupaten mungkin memiliki data yang kosong (null). [cite: 57]
    * **Accuracy**: Cukup Tinggi. [cite_start]Berdasarkan hasil penimbangan riil di TPS/TPA sebelum dikalkulasi persentase kebocorannya. [cite: 58]
    * **Consistency**: Tinggi. [cite_start]Kategori komposisi sampah (Plastik, Kertas, Logam) menggunakan standar nasional yang sama dari tahun ke tahun. [cite: 59]
    * [cite_start]**Timeliness**: Dirilis pada tahun berikutnya setelah semua daerah selesai merekapitulasi laporan tahunan. [cite: 60]

### [cite_start]3.2 Dataset Kaggle [cite: 61]
* [cite_start]**Dataset Name**: Water and Air Quality (Numbeo Indices) [cite: 63]
* [cite_start]**Creator/Publisher**: Patrick L. Ford [cite: 66]
* [cite_start]**URL/Access Point**: https://www.kaggle.com/datasets/patricklford/water-and-air-quality [cite: 64, 65]
* [cite_start]**Format Data**: CSV [cite: 69]
* [cite_start]**Data Quality**: [cite: 79]
    * **Missing Values**: Low (<5%). [cite_start]Sebagian besar metrik lengkap untuk kota-kota besar yang terdaftar. [cite: 80]
    * **Consistency**: Medium. Membutuhkan proses filtering wilayah yang ketat. [cite_start]Kolom Country harus disaring hanya untuk 'Indonesia', dan data City harus dicocokkan (di-mapping) secara manual agar hanya menyisakan kota-kota pesisir yang relevan dengan data populasi laut (seperti Jakarta, Surabaya, Denpasar). [cite: 82]
    * **Documentation Quality**: Cukup. [cite_start]Metrik didasarkan pada survei persepsi dan agregasi Numbeo, sehingga sifat datanya adalah indeks kualitatif yang dikuantifikasi (bukan volume fisik polutan). [cite: 83]

### [cite_start]3.3 Public APIs [cite: 84]
* [cite_start]**API Name**: OBIS API (Ocean Biodiversity Information System [cite: 86]
* [cite_start]**Provider**: UNESCO - Intergovernmental Oceanographic Commission (IOC) Authentication Method: Open Access (No API Key required) [cite: 88]
* [cite_start]**Endpoint URL**: https://api.obis.org [cite: 87]
* [cite_start]**Response Format**: JSON [cite: 90]
* [cite_start]**Rate Limits**: Fleksibel (Disarankan tidak lebih dari 10 request per detik) [cite: 91]
* [cite_start]**Cost**: Free (Open Data) [cite: 93]
* [cite_start]**Reliability**: Sangat Tinggi (Digunakan oleh komunitas periset global) [cite: 92]

### [cite_start]3.4 Open Research Data [cite: 94]
* [cite_start]**Dataset Name**: Global Marine Debris Dataset [cite: 96]
* [cite_start]**Repository**: PANGAEA - Data Publisher for Earth & Environmental Science Research Institution: https://www.pangaea.de/ [cite: 97]
* [cite_start]**Publication Date**: Alfred Wegener Institute for Polar and Marine Research & International Marine Debris Research Community [cite: 98]