# Analisis Pengaruh Sampah Laut terhadap Populasi Makhluk Hidup Laut

## 1. Executive Summary

**Project Overview**
* **Tujuan Project**: Penelitian ini bertujuan untuk menganalisis pengaruh sampah laut terhadap populasi makhluk hidup laut dengan mengidentifikasi hubungan antara tingkat pencemaran sampah dan perubahan jumlah populasi organisme laut dari waktu ke waktu.
* **Fokus Penelitian**: Penelitian ini juga bertujuan untuk mengetahui jenis sampah yang paling dominan serta spesies yang paling terdampak oleh pencemaran tersebut. Melalui pendekatan analisis data dan visualisasi statistik, diharapkan penelitian ini dapat memberikan gambaran mengenai sejauh mana sampah laut memengaruhi keseimbangan ekosistem laut serta menjadi dasar dalam upaya pengelolaan dan pengendalian pencemaran lingkungan laut.
* **Scope Project**: Ruang lingkup project ini mencakup integrasi data jumlah sampah laut, khususnya sampah plastik dan mikroplastik, dengan data populasi makhluk hidup laut pada periode waktu tertentu. Data yang digunakan meliputi volume atau tingkat pencemaran sampah laut, jumlah populasi spesies laut, serta informasi wilayah perairan yang dianalisis. Project ini berfokus pada analisis hubungan antara tingkat pencemaran dan perubahan populasi menggunakan metode statistik dan visualisasi data, tanpa melakukan pengambilan data lapangan secara langsung.
* **Timeline**: 3 Bulan (Februari - Mei)

**Expected Outcomes**:
* Insight mengenai hubungan antara tingkat sampah laut dan perubahan populasi makhluk hidup laut
* Identifikasi spesies yang paling terdampak pencemaran
* Visualisasi tren pencemaran dan penurunan populasi per wilayah/periode waktu
* Model Machine Learning untuk memprediksi dampak peningkatan sampah plastik terhadap populasi biota laut
* Klasifikasi wilayah pesisir berdasarkan tingkat risiko ekologis
* Rekomendasi berbasis data untuk pengelolaan dan pengurangan sampah laut

---

## 2. Stakeholders

* **Project Owner**: Kementerian Kelautan dan Perikanan (KKP)
    * Pemerintah Daerah (wilayah pesisir)
    * Kementerian Kelautan dan Perikanan
    * Dinas Lingkungan Hidup

### Team Members

| Nama | NIM | Role |
| :--- | :--- | :--- |
| **Arie Dwi Sulistyo**  | (244311004)  | Project Manager  |
| **Muhammad Rofiqul A.**  | (244311019)  | Data Engineer  |
| **Dila Alif Regita**  | (244311010)  | Data Analyst |
| **Suqya Rohmatin**  | (244311028)  | Data Analyst |

> **Dosen Pengampu**: Gus Nanang Syaifuddiin, S.Kom., M.Kom.
> **Program Studi**: TRPL, JURUSAN TEKNIK
> **Institusi**: POLITEKNIK NEGERI MADIUN 2026

---

## 3. Data Source Analysis

### 3.1 Data Pemerintah (data.go.id)
* **Dataset Name**: Timbulan Sampah dan Komposisi Sampah (Fokus Wilayah Pesisir/Kabupaten)
* **Data Owner**: Kementerian Lingkungan Hidup dan Kehutanan (KLHK)
* **URL/Access Point**: https://sipsn.menlhk.go.id/sipsn/ & https://data.go.id/
* **Update Frequency**: Semesteran / Tahunan
* **Time Coverage**: 2015 - 2024
* **Format Data**: CSV, Excel, Web Dashboard
* **Data Quality**:
    * **Completeness**: Medium (~70-80%). Bergantung pada kepatuhan pelaporan masing-masing pemerintah daerah. Beberapa kabupaten mungkin memiliki data yang kosong (null).
    * **Accuracy**: Cukup Tinggi. Berdasarkan hasil penimbangan riil di TPS/TPA sebelum dikalkulasi persentase kebocorannya.
    * **Consistency**: Tinggi. Kategori komposisi sampah (Plastik, Kertas, Logam) menggunakan standar nasional yang sama dari tahun ke tahun.
    * **Timeliness**: Dirilis pada tahun berikutnya setelah semua daerah selesai merekapitulasi laporan tahunan.

### 3.2 Dataset Kaggle 
* **Dataset Name**: Water and Air Quality (Numbeo Indices)
* **Creator/Publisher**: Patrick L. Ford
* **URL/Access Point**: https://www.kaggle.com/datasets/patricklford/water-and-air-quality
* **Format Data**: CSV
* **Data Quality**:
    * **Missing Values**: Low (<5%). Sebagian besar metrik lengkap untuk kota-kota besar yang terdaftar.
    * **Consistency**: Medium. Membutuhkan proses filtering wilayah yang ketat. Kolom Country harus disaring hanya untuk 'Indonesia', dan data City harus dicocokkan (di-mapping) secara manual agar hanya menyisakan kota-kota pesisir yang relevan dengan data populasi laut (seperti Jakarta, Surabaya, Denpasar).
    * **Documentation Quality**: Cukup. Metrik didasarkan pada survei persepsi dan agregasi Numbeo, sehingga sifat datanya adalah indeks kualitatif yang dikuantifikasi (bukan volume fisik polutan).

### 3.3 Public APIs
* **API Name**: OBIS API (Ocean Biodiversity Information System
* **Provider**: UNESCO - Intergovernmental Oceanographic Commission (IOC) Authentication Method: Open Access (No API Key required)
* **Endpoint URL**: https://api.obis.org
* **Response Format**: JSON
* **Rate Limits**: Fleksibel (Disarankan tidak lebih dari 10 request per detik)
* **Cost**: Free (Open Data)
* **Reliability**: Sangat Tinggi (Digunakan oleh komunitas periset global)

### 3.4 Open Research Data
* **Dataset Name**: Global Marine Debris Dataset
* **Repository**: PANGAEA - Data Publisher for Earth & Environmental Science Research Institution: https://www.pangaea.de/
* **Publication Date**: Alfred Wegener Institute for Polar and Marine Research & International Marine Debris Research Community