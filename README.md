# Prediksi Tingkat Kerusakan Bangunan Pasca Gempa Berdasarkan Jenis Material Bangunan

## 1. Project Information
* **Project Name:** Prediksi Tingkat Kerusakan Bangunan Pasca Gempa Berdasarkan Jenis Material Bangunan
* **Created By:** Kelompok 2
* **Date:** February 19, 2026
* **Version:** 1.0

## 2. Executive Summary
### 2.1. Project Overview
* **Tujuan Project:** Mengembangkan model Machine Learning untuk memprediksi tingkat kerusakan infrastruktur bangunan berdasarkan parameter seismik dan karakteristik struktur fisik bangunan.
* **Scope Project:** Integrasi data historis gempa BMKG/USGS dan analisis data teknis bangunan (usia, material, tinggi) untuk mengklasifikasikan skala kerusakan.
* **Expected Outcomes:** Model prediksi tingkat kerusakan berdasarkan damage grade (Skala 1-3) dan laporan analisis pengaruh jenis material terhadap ketahanan bencana.
* **Timeline:** (Maret - Juni 2026).

### 2.2. Stakeholders
* **Project Owner:** BMKG & BNPB (Badan Nasional Penanggulangan Bencana).
* **Team Members:**
1. **Project Manager:** Kevin Rafael Suryatmoko
2. **Data Engineer:** Muhammad Rifqi Maulana
3. **Data Analyst:** Fathur Roshin Haddinanta
* **End Users:** Pemerintah Daerah, Perusahaan Konstruksi, dan Asuransi.

## 3. Data Source Analysis
### 3.1. Data Pemerintah (BMKG)
* **Dataset Name:** Katalog Gempa Bumi Terintegrasi Indonesia.
* **URL/Access Point:** https://repogempa.bmkg.go.id/eventcatalog
* **Format Data:** CSV, EXCEL, PDF.
* **Volume Data:** Lebih dari 100.000 baris.
* **Time Coverage:** 2008 - Sekarang.
* **Kualitas Data:** Kelengkapan 100%, akurasi tinggi (data resmi pemerintah), dan diperbarui secara harian.

### 3.2. Dataset Kaggle
* **Dataset Name:** Richter's Predictor: Modeling Earthquake Damage.
* **URL/Access Point:** https://www.kaggle.com/datasets/mullerismail/richters-predictor-modeling-earthquake-damage
* **Format Data:** CSV (23.44MB).
* **Volume Data:** 260.601 baris.
* **Fitur Utama:** building_id, geo_level, count_floors_pre_eq, age, area_percentage, height_percentage, land_surface_condition, foundation_type, has_superstructure.
* **Metrik Kualitas:** Missing values rendah, konsistensi baik, dan bersumber dari National Planning Commission.

### 3.3. Public APIs (USGS)
* **API Name:** USGS Earthquake Catalog API.
* **Endpoint:** https://earthquake.usgs.gov/fdsnws/event/1/query?format=geojson&starttime=2015-01-01&endtime=2015-12-31&minmagnitude=7
* **Parameter:** format (struktur data), starttime (waktu mulai), endtime (waktu selesai), mag (magnitudo).
* **Keunggulan API:** Reliabilitas sangat tinggi (standar global), dokumentasi lengkap, akses gratis (Open Access).
