Analisis Prediktif Emisi CO₂ di Spanyol (2010–2022)
Background / Problem Statement
Emisi karbon dioksida (CO₂) adalah salah satu faktor utama dalam perubahan iklim global. Sebagai negara dengan ekonomi yang berkembang pesat di Eropa, Spanyol menghadapi tantangan besar dalam mengelola emisi karbon dari sektor industri, energi, dan transportasi.

Proyek ini bertujuan untuk menganalisis tren emisi CO₂ di Spanyol selama 2010–2022, mengidentifikasi faktor-faktor utama yang mempengaruhi emisi, serta memprediksi tingkat emisi di masa depan menggunakan pendekatan pembelajaran mesin (machine learning). Hasil analisis ini diharapkan dapat memberikan wawasan untuk mendukung kebijakan keberlanjutan dan efisiensi energi.

What is in the Project
Proyek ini mencakup langkah-langkah berikut:

Data Understanding:
Menggunakan dataset publik dari Our World in Data dan sumber lainnya.
Melakukan eksplorasi variabel seperti intensitas energi, pajak lingkungan, dan konsumsi energi per kapita.
Data Preparation:
Membersihkan data, menangani nilai hilang, dan melakukan transformasi variabel.
Menggunakan teknik seperti SMOTE untuk menangani ketidakseimbangan data.
Modeling:
Membangun model prediktif menggunakan Random Forest Regression dan membandingkannya dengan model lain seperti K-Nearest Neighbors.
Melakukan hyperparameter tuning dengan GridSearchCV untuk meningkatkan akurasi model.
Evaluation:
Mengevaluasi model menggunakan metrik seperti R², RMSE, dan MAE.
Menginterpretasi hasil dengan analisis feature importance untuk memahami variabel yang paling memengaruhi emisi CO₂.
Machine Learning Model Result
Model yang Digunakan:
Random Forest Regression dipilih karena kinerjanya yang baik dalam menangkap hubungan non-linear dan toleransi terhadap fitur yang tidak relevan.
Evaluasi Model:
R²: 92.7% – Menunjukkan bahwa model dapat menjelaskan sebagian besar variabilitas dalam data.
RMSE: 0.17% – Error prediksi model cukup rendah.
Feature Importance: Variabel seperti pajak kendaraan (ENVTAX_VEH), emisi berbasis produksi (CO2_PBEM), dan intensitas energi (NRG_INT) menjadi faktor paling signifikan dalam memengaruhi prediksi.
Visualisasi Hasil:
Grafik tren prediksi menunjukkan kesesuaian antara data aktual dan hasil prediksi, terutama dalam tren penurunan emisi CO₂ setelah 2017.
Conclusion
Proyek ini menunjukkan bahwa pendekatan berbasis data dapat memberikan wawasan yang mendalam tentang faktor-faktor utama yang memengaruhi emisi karbon. Model prediktif seperti Random Forest Regression dapat digunakan untuk membantu pemerintah dan pembuat kebijakan:

Mengidentifikasi sektor yang perlu dioptimalkan untuk pengurangan emisi karbon.
Mendukung inisiatif keberlanjutan, seperti transisi ke energi terbarukan dan kebijakan pajak lingkungan yang lebih efektif.
Memantau tren emisi di masa depan untuk memastikan bahwa target pengurangan emisi global dapat tercapai.
Melalui pendekatan sistematis ini, analisis prediktif memberikan kontribusi nyata dalam menciptakan masa depan yang lebih hijau dan berkelanjutan.


