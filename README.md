# 🍫 Global Chocolate Sales Analysis & Forecast 2025

![Python](https://img.shields.io/badge/Python-3.x-blue?style=flat&logo=python)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange?style=flat&logo=jupyter)
![Machine Learning](https://img.shields.io/badge/Machine-Learning-red?style=flat)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=flat)

## 🤔 Latar Belakang Bisnis
Di industri ritel yang dinamis, memahami perilaku konsumen dan memprediksi pendapatan adalah kunci untuk menjaga ketersediaan stok dan mengoptimalkan margin. Proyek ini bertujuan untuk membongkar data transaksi penjualan cokelat global sepanjang tahun 2025 untuk menggali informasi strategis.

## 🎯 Tujuan
Proyek analisis ini digerakkan oleh dua tujuan utama:
1. **Sales Prediction:** Memprediksi total `Revenue_USD` dari sebuah transaksi menggunakan model regresi agar tim *finance* dapat melakukan *forecasting* dengan lebih akurat.
2. **Customer Segmentation:** Mengelompokkan pola pembelian menggunakan metode *K-Means clustering* untuk membantu tim *marketing* mendesain promosi yang tepat sasaran.

## 📊 Informasi Dataset
Proyek ini menggunakan dataset `chocolate_sales_2025_dataset.csv` yang berisi riwayat 500 transaksi. Fitur data yang dianalisis meliputi:
* `Sale_ID`: ID unik transaksi.
* `Date`: Tanggal transaksi penjualan.
* `Brand` & `Product_Type`: Merek (misalnya Lindt, Ferrero, Cadbury) dan jenis produk.
* `Country`: Negara tempat transaksi berlangsung.
* `Sales_Channel` & `Payment_Method`: Jalur distribusi dan metode pembayaran konsumen.
* `Price_USD`, `Units_Sold`, `Revenue_USD`: Angka pengukur metrik finansial.

## 🛠️ Metodologi & Langkah Kerja
**Tahap A: Data Preprocessing & Exploratory Data Analysis (EDA)**
* Melakukan pengecekan kualitas data dan kekosongan data (*missing values*).
* Menggali informasi waktu tambahan dengan mengekstrak fitur bulan dari kolom `Date` agar dapat diserap oleh algoritma *Machine Learning*.
* Melakukan analisis tren penjualan bulanan dan mengidentifikasi merek penyumbang pendapatan tertinggi.
* Visualisasi *Correlation Heatmap* antar fitur numerik.

**Tahap B: Customer Segmentation (Clustering)**
* Melakukan standarisasi atau normalisasi pada fitur-fitur numerik yang akan digunakan untuk *clustering*.
* Menentukan jumlah *cluster* (kelompok) yang optimal menggunakan metode evaluasi seperti *Silhouette Score*.
* Melatih model *K-Means Clustering* untuk membagi pelanggan ke dalam 3 segmen utama.

**Tahap C: Sales Prediction (Regression)**
* Menyiapkan data untuk pemodelan (misalnya melakukan *encoding* pada data kategorikal dan membagi data menjadi *Training* serta *Testing set*).
* Membangun dan melatih model *Machine Learning* berbasis regresi untuk memprediksi angka `Revenue_USD` dari setiap transaksi.
* Melakukan evaluasi performa model untuk memastikan tingkat akurasi prediksi.

## ✨ Hasil & Actionable Insights
* Berdasarkan metode evaluasi *Silhouette Score* dan interpretasi kebutuhan bisnis, karakteristik pelanggan berhasil dipetakan ke dalam 3 Cluster utama.
* Buka notebook untuk melihat karakteristik seluruh segmen dan hasil prediksi.
