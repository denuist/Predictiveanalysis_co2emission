# 🔍 Analisis Prediktif Penghasil Emisi CO₂ Berbasis Industri dan Ekonomi di Spanyol (2010–2022)

## 📜 Background / Problem Statement
Emisi karbon dioksida (CO₂) adalah salah satu faktor utama dalam perubahan iklim global. Sebagai negara dengan ekonomi yang berkembang pesat di Eropa, Spanyol menghadapi tantangan besar dalam mengelola emisi karbon dari sektor industri, energi, dan transportasi.

Project ini bertujuan untuk menganalisis tren emisi CO₂ di Spanyol selama 2010–2022, mengidentifikasi faktor-faktor utama yang mempengaruhi emisi, serta memprediksi tingkat emisi di masa depan menggunakan pendekatan pembelajaran mesin (*machine learning*). Hasil analisis ini diharapkan dapat memberikan wawasan untuk mendukung kebijakan keberlanjutan dan efisiensi energi.

## 📊 Dataset
Dataset utama diambil dari real dataset yang bersumber pada https://data-explorer.oecd.org/. dengan cakupan waktu dari tahun 2010 - 2022 dengan referensi Negara Spanyol

## 🌐 Dashboard Link
(https://lookerstudio.google.com/reporting/10db9fac-35bb-42b5-b9b7-21a660affd7d)

## 📋 File Requirements
pandas: Digunakan untuk manipulasi dan analisis data.
numpy: Digunakan untuk operasi numerik.
matplotlib: Untuk membuat visualisasi.
scipy: Digunakan untuk operasi statistik (stats module).
seaborn: Membuat visualisasi data yang lebih canggih.
scikit-learn: Untuk model machine learning, preprocessing, dan evaluasi.
imbalanced-learn: Untuk menangani data imbalance, misalnya SMOTE.
statsmodels: Untuk analisis statistik seperti Variance Inflation Factor (VIF).

## 📌 What is in the Project
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

## 🤖  Machine Learning Model Result

### Model yang Digunakan
*Random Forest Regression* dipilih karena kinerjanya yang baik dalam menangkap hubungan non-linear dan toleransi terhadap fitur yang tidak relevan.

### Evaluasi Model
Setelah melakukan *hyperparameter tuning* pada kedua model, berikut adalah hasil evaluasi yang diperoleh untuk masing-masing model:

- **Random Forest**:
  - **R²**: 92.7%
  - **RMSE**: 0.17%
  - **MAE**: 0.12

- **KNN**:
  - **R²**: 85.3%
  - **RMSE**: 0.23%
  - **MAE**: 0.15

### 🔮 Insight
- **Random Forest** menunjukkan performa yang lebih baik setelah *hyperparameter tuning*, dengan **R²** yang lebih tinggi dan **RMSE** yang lebih rendah.
- **KNN** meskipun cukup baik, memiliki performa yang lebih rendah dalam hal kemampuan untuk menjelaskan variabilitas data jika dibandingkan dengan *Random Forest*.
  
### Feature Importance
Variabel yang paling berpengaruh dalam memprediksi emisi CO₂:
  - Pajak kendaraan: `ENVTAX_VEH`
  - Emisi berbasis produksi: `CO2_PBEM`
  - Intensitas energi: `NRG_INT`

## Visualisasi Hasil

### **Perbandingan antara model Random Forest dan KNN untuk evaluasi kinerja berdasarkan metrik utama.**
<img width="500" alt="Random forest Regressor after Tuned" src="https://github.com/user-attachments/assets/b8a3c952-dc83-4144-aa1a-0b5a600700c8" /> <img width="500" alt="KNN after Tuned" src="https://github.com/user-attachments/assets/28c75acb-076b-43cb-a278-4c6e984e0a3a" />
<img width="500" alt="KNN after Tuned" src="https://github.com/user-attachments/assets/28c75acb-076b-43cb-a278-4c6e984e0a3a" />

### **Grafik tren prediksi menunjukkan kesesuaian antara data aktual dan hasil prediksi, terutama dalam tren penurunan emisi CO₂ setelah 2017.**
<img width="1000" alt="gambar data aktual vs prediksi" src="https://github.com/user-attachments/assets/a92857f9-c809-4472-bfff-50d8a895a188" />

## ✅ Conclusion
Project ini menunjukkan bahwa pendekatan berbasis data dapat memberikan wawasan yang mendalam tentang faktor-faktor utama yang memengaruhi emisi karbon. Model prediktif seperti *Random Forest Regression* dapat digunakan untuk membantu pemerintah dan pembuat kebijakan:

1. Mengidentifikasi sektor yang perlu dioptimalkan untuk pengurangan emisi karbon.
2. Mendukung inisiatif keberlanjutan, seperti transisi ke energi terbarukan dan kebijakan pajak lingkungan yang lebih efektif.
3. Memantau tren emisi di masa depan untuk memastikan bahwa target pengurangan emisi global dapat tercapai.

Melalui pendekatan sistematis ini, analisis prediktif memberikan kontribusi nyata dalam menciptakan masa depan yang lebih hijau dan berkelanjutan.



