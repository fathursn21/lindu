# Prediksi Tingkat Kerusakan Bangunan Pasca Gempa

Proyek ini bertujuan untuk mengembangkan model *Machine Learning* yang mampu memprediksi tingkat kerusakan infrastruktur bangunan (Damage Grade 1-3) berdasarkan parameter seismik dan karakteristik fisik bangunan.

## 📋 Tentang Proyek
Proyek ini diinisiasi untuk memberikan kontribusi pada mitigasi bencana dengan memanfaatkan data teknis bangunan dan data historis gempa dari BMKG serta sumber global.

- **Nama Proyek:** Prediksi Tingkat Kerusakan Bangunan Pasca Gempa Berdasarkan Jenis Material Bangunan
- **Versi:** 1.0
- **Timeline:** Maret - Mei 2026
- **Stakeholder:** BMKG & BNPB

## 👥 Tim Pengembang
| Peran | Nama |
| :--- | :--- |
| **Project Manager** | Kevin Rafael Suryatmoko |
| **Data Engineer** | Muhammad Rifqi Maulana |
| **Data Analyst** | Fathur Roshin Haddinanta |

## 📊 Sumber Data
Proyek ini mengintegrasikan data dari berbagai sumber untuk memastikan akurasi model:

1. **Katalog Gempa Bumi Indonesia (BMKG)**
   - **Tipe:** Data Seismik (CSV, JSON, XML)
   - **Cakupan:** 2008 - Sekarang
   - **Sumber:** [data.bmkg.go.id](https://data.bmkg.go.id/gempabumi/)

2. **Richter's Predictor (Kaggle)**
   - **Tipe:** Data Karakteristik Bangunan
   - **Detail:** > 260.000 baris data mengenai struktur fisik (usia, material, tinggi, dll.)
   - **Sumber:** [Kaggle Dataset](https://www.kaggle.com/datasets/mullerismail/richters-predictor-modeling-earthquake-damage)
