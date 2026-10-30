📊 Prediksi Angka Buta Huruf di Jawa Barat Menggunakan Regresi Linear Berganda

Repositori ini berisi proyek analisis data dan pemodelan prediktif untuk memprediksi Angka Buta Huruf di kabupaten/kota Provinsi Jawa Barat berdasarkan indikator demografi dan sosial-ekonomi.

📌 Ringkasan Proyek

Proyek ini bertujuan untuk menganalisis tren sosial serta membangun model pembelajaran mesin (machine learning) guna memprediksi Angka Buta Huruf hingga 3 tahun mendatang (2024–2026).

Metodologi mencakup:

Exploratory Data Analysis (EDA): Pembersihan data (data cleansing) dan analisis deskriptif terhadap 189 entitas data kabupaten/kota.

Optimasi Hyperparameter Sederhana: Eksperimen iteratif pencarian random_state terbaik untuk mengoptimalkan evaluasi metrik $R^2$ (R-Squared).

Pemodelan Regresi Linear Berganda: Menggunakan fitur Jumlah Penduduk, Jumlah SD, dan Persentase Penduduk Miskin untuk memprediksi target Angka Buta Huruf.

Prediksi Masa Depan (3-Year Forecasting): Memprediksi tren pertumbuhan indikator pendukung serta nilai Angka Buta Huruf untuk periode 2024–2026.

🛠️ Teknologi & Library yang Digunakan

Bahasa Pemrograman: Python 3

Manipulasi Data: pandas, numpy

Machine Learning & Statistik: scikit-learn (LinearRegression, train_test_split, r2_score, mean_absolute_error, mean_squared_error)

📂 Struktur Dataset (Project1.xlsx)

Dataset memuat 189 baris data histori (2017–2023) dengan fitur-fitur berikut:

Kota/Kabupaten & Tahun (Variabel Identitas)

Jumlah Penduduk (Fitur / $X_1$)

Jumlah SD (Fitur / $X_2$)

Presentase Penduduk Miskin (Fitur / $X_3$)

Angka Buta Huruf (Target / $Y$)

📈 Evaluasi Model & Hasil Utama

1. Evaluasi Model Prediksi

| Metrik Evaluasi | Nilai | Keterangan / Interpretasi |
| :--- | :---: | :--- |
| **Best Random State** | `36789` | Titik acuan *split* data optimal terbaik |
| **R-Squared (R²)** | `0.5801` | Model mampu menjelaskan ~58% variansi target |
| **MAE (Mean Absolute Error)** | `0.5780` | Rata-rata tingkat kesalahan absolut prediksi |
| **MSE (Mean Squared Error)** | `0.6049` | Rata-rata kuadrat error dari model regresi |

2. Proyeksi Angka Buta Huruf (2024 – 2026)

| Tahun | Prediksi Angka Buta Huruf (%) |
| :---: | :---: |
| 2024 | 1.311% |
| 2025 | 1.327% |
| 2026 | 1.344% |

🚀 Cara Menjalankan Notebook

Clone repositori ini ke komputer Anda:

git clone https://github.com/NitaaSF/prediksi_Angka_Buta_Huruf



Pastikan dependensi terinstal:

pip install pandas numpy scikit-learn openpyxl



Buka file .ipynb menggunakan Jupyter Notebook, VS Code, atau unggah ke Google Colab.

Dikembangkan oleh Nita Sawalia Fitri
