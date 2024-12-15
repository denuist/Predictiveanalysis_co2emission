# Analisis Prediktif Penghasil Emisi CO₂ Berbasis Industri dan Ekonomi di Spanyol (2010–2022)

## Background / Problem Statement
Emisi karbon dioksida (CO₂) adalah salah satu faktor utama dalam perubahan iklim global. Sebagai negara dengan ekonomi yang berkembang pesat di Eropa, Spanyol menghadapi tantangan besar dalam mengelola emisi karbon dari sektor industri, energi, dan transportasi.

Project ini bertujuan untuk menganalisis tren emisi CO₂ di Spanyol selama 2010–2022, mengidentifikasi faktor-faktor utama yang mempengaruhi emisi, serta memprediksi tingkat emisi di masa depan menggunakan pendekatan pembelajaran mesin (*machine learning*). Hasil analisis ini diharapkan dapat memberikan wawasan untuk mendukung kebijakan keberlanjutan dan efisiensi energi.

## Dataset
Dataset utama diambil dari real dataset yang bersumber pada https://data-explorer.oecd.org/. dengan cakupan waktu dari tahun 2010 - 2022 dengan referensi Negara Spanyol

## Dashboard Link
(https://lookerstudio.google.com/reporting/10db9fac-35bb-42b5-b9b7-21a660affd7d)

## File Requirements
pandas: Digunakan untuk manipulasi dan analisis data.
numpy: Digunakan untuk operasi numerik.
matplotlib: Untuk membuat visualisasi.
scipy: Digunakan untuk operasi statistik (stats module).
seaborn: Membuat visualisasi data yang lebih canggih.
scikit-learn: Untuk model machine learning, preprocessing, dan evaluasi.
imbalanced-learn: Untuk menangani data imbalance, misalnya SMOTE.
statsmodels: Untuk analisis statistik seperti Variance Inflation Factor (VIF).

## What is in the Project
Proyek ini mencakup langkah-langkah berikut:

### 1. **Data Understanding**
   - Menggunakan dataset publik dari *Our World in Data* dan sumber lainnya.
   - Melakukan eksplorasi variabel seperti intensitas energi, pajak lingkungan, dan konsumsi energi per kapita.

### 2. **Data Preparation**
   - Membersihkan data, menangani nilai hilang, dan melakukan transformasi variabel.
   - Menggunakan teknik seperti *SMOTE* untuk menangani ketidakseimbangan data.

### 3. **Modeling**
   - Membangun model prediktif menggunakan *Random Forest Regression* dan membandingkannya dengan model lain seperti *K-Nearest Neighbors*.
   - Melakukan *hyperparameter tuning* dengan *GridSearchCV* untuk meningkatkan akurasi model.

### 4. **Evaluation**
   - Mengevaluasi model menggunakan metrik seperti R², RMSE, dan MAE.
   - Menginterpretasi hasil dengan analisis *feature importance* untuk memahami variabel yang paling memengaruhi emisi CO₂.

## Machine Learning Model Result

### Model yang Digunakan
*Random Forest Regression* dipilih karena kinerjanya yang baik dalam menangkap hubungan non-linear dan toleransi terhadap fitur yang tidak relevan.

### Evaluasi Model
- **R²**: 92.7% – Menunjukkan bahwa model dapat menjelaskan sebagian besar variabilitas dalam data.
- **RMSE**: 0.17% – Error prediksi model cukup rendah.
  
### Feature Importance
Variabel yang paling berpengaruh dalam memprediksi emisi CO₂:
  - Pajak kendaraan: `ENVTAX_VEH`
  - Emisi berbasis produksi: `CO2_PBEM`
  - Intensitas energi: `NRG_INT`

### Visualisasi Hasil
Grafik tren prediksi menunjukkan kesesuaian antara data aktual dan hasil prediksi, terutama dalam tren penurunan emisi CO₂ setelah 2017.
![gambar data aktual vs prediksi](https://github.com/user-attachments/assets/a92857f9-c809-4472-bfff-50d8a895a188)


## Conclusion
Project ini menunjukkan bahwa pendekatan berbasis data dapat memberikan wawasan yang mendalam tentang faktor-faktor utama yang memengaruhi emisi karbon. Model prediktif seperti *Random Forest Regression* dapat digunakan untuk membantu pemerintah dan pembuat kebijakan:

1. Mengidentifikasi sektor yang perlu dioptimalkan untuk pengurangan emisi karbon.
2. Mendukung inisiatif keberlanjutan, seperti transisi ke energi terbarukan dan kebijakan pajak lingkungan yang lebih efektif.
3. Memantau tren emisi di masa depan untuk memastikan bahwa target pengurangan emisi global dapat tercapai.

Melalui pendekatan sistematis ini, analisis prediktif memberikan kontribusi nyata dalam menciptakan masa depan yang lebih hijau dan berkelanjutan.



