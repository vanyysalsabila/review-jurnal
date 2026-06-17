# 📚 Kumpulan Review Jurnal: Prediksi Kualitas Udara Menggunakan Machine Learning

Repositori ini berisi ringkasan dan poin-poin penting dari 24 jurnal ilmiah terkait prediksi Air Quality Index (AQI) dan polutan udara menggunakan berbagai pendekatan *Machine Learning* dan *Deep Learning*.

---

## 📋 Daftar Review Jurnal

### 1. Global Air Quality Index Prediction Using Machine Learning on Major Pollutants
- **Fokus Utama**: Memprediksi AQI global berdasarkan polutan utama (PM2.5, O3, NO2, CO) menggunakan model regresi (Linear Regression, SVR, Random Forest, XGBoost, LightGBM).
- **Poin Penting**:
  - XGBoost merupakan model dengan performa terbaik dan paling stabil (R² 0.9971).
  - PM2.5 adalah polutan paling berpengaruh terhadap nilai AQI global.
  - Dilengkapi dengan *dashboard interaktif* untuk memvisualisasikan prediksi AQI berbagai negara.

### 2. Unleashing Realistic Air Quality Forecasting: Introducing the Ready-to-Use PurpleAirSF Dataset
- **Fokus Utama**: Memperkenalkan dataset open-source baru bernama *PurpleAirSF* yang diambil dari jaringan PurpleAir untuk mendukung riset prediksi kualitas udara.
- **Poin Penting**:
  - Dataset ini memiliki resolusi temporal tinggi dan cakupan geografis yang beragam.
  - Dapat digunakan sebagai *benchmark* untuk model prediksi spatio-temporal (klasik maupun modern).

### 3. Air Quality Forecasting Using Machine Learning: A Global perspective with Relevance to Low-Resource Settings
- **Fokus Utama**: Prediksi kualitas udara yang dioptimalkan untuk negara berpendapatan rendah (keterbatasan sumber daya) menggunakan data World Weather Repository dari 197 ibu kota negara.
- **Poin Penting**:
  - Random Forest sangat efektif, terutama saat diterapkan untuk tugas klasifikasi daripada regresi (akurasi meningkat 42%).
  - Mengedepankan Explainable AI (XAI) agar prediksi mudah dipahami, serta mempertimbangkan analisis efisiensi biaya (*cost-effectiveness*).

### 4. Improving Local Air Quality Predictions Using Transfer Learning on Satellite Data and Graph Neural Networks
- **Fokus Utama**: Menggunakan *Transfer Learning* dengan GNN (GraphSAGE) dan data satelit untuk memprediksi kadar NO2 di lokasi yang tidak memiliki stasiun pemantauan (sensor virtual).
- **Poin Penting**:
  - Model yang di-*pre-train* di London terbukti berhasil meningkatkan akurasi prediksi di Bristol (penurunan NRMSE 8.6%).
  - Membantu monitoring wilayah dengan *data-scarce* secara hemat biaya.

### 5. Air Quality PM2.5 Index Prediction Model Based on CNN - LSTM
- **Fokus Utama**: Model hibrida CNN-LSTM untuk memprediksi PM2.5 rata-rata tiap 6 jam di area industri Beijing.
- **Poin Penting**:
  - CNN digunakan untuk ekstraksi fitur spasial, sementara LSTM untuk pola temporal (*time-series*).
  - Berhasil mengungguli model *time-series* tradisional untuk sistem peringatan dini polusi udara industri.

### 6. Machine Learning Models for Advanced Air Quality Prediction
- **Fokus Utama**: Membandingkan Random Forest Regression (RFR) dan LSTM untuk prediksi PM2.5 di kota Bishkek, Kyrgyzstan yang sering mengalami masalah kabut asap tebal (*smog*) di musim dingin.
- **Poin Penting**:
  - RFR memberikan hasil yang lebih unggul dibandingkan LSTM dengan akurasi mencapai 90%.
  - Faktor cuaca sangat berperan dalam akurasi prediksi tingkat keparahan PM2.5.

### 7. Transforming Air Quality Index Prediction Using ML: Insights from Taj Trapezium Zone (TTZ)
- **Fokus Utama**: Memprediksi AQI di area Taj Mahal (TTZ, Agra, India) untuk membantu mengantisipasi *Graded Response Action Plan* (GRAP).
- **Poin Penting**:
  - Menggunakan algoritma *ensemble*: AdaBoost, XGBoost, CatBoost, dan LightGBM.
  - Sangat berguna untuk pemerintah setempat dalam mencegah kerugian ekonomi yang ditimbulkan oleh penerapan GRAP mendadak tanpa prediksi yang baik.

### 8. Next-Gen Air Quality Index Forecasting with Hybrid Machine Learning Models and Cloud Synergy
- **Fokus Utama**: Model prediktif yang menggabungkan Convolutional Neural Networks (CNN) dengan arsitektur Transformer dan *Attention Mechanism* di lingkungan *Cloud computing*.
- **Poin Penting**:
  - Menyelesaikan kelemahan model deret waktu jadul seperti ARIMA/LSTM untuk mengekstrak korelasi spasial-temporal kompleks.
  - Mendukung *streaming* data sensor langsung secara *real-time* berkat sinergi komputasi awan.

### 9. Forecasting the Air Quality Index Using Machine Learning Models, Bayesian Optimization, and the Development of the S-GBR Model Incorporating Seasonal Variables
- **Fokus Utama**: Memperkenalkan *Seasonal Gradient Boosting Regressor (S-GBR)* dengan pengoptimalan parameter tipe *Bayesian Optimization*.
- **Poin Penting**:
  - Mengatasi masalah utama model ML yang sering melupakan variabel musim/waktu.
  - Penambahan input *seasonal* dan optimasi hyperparameter dengan Bayesian memberikan akurasi jauh di atas nilai *default*.

### 10. Application of the XGBoost Machine Learning Method in PM2.5 Prediction: A Case Study of Shanghai
- **Fokus Utama**: Pemanfaatan algoritma XGBoost dipadukan dengan output dari model sistem prediksi numerik atmosfer WRF-Chem untuk wilayah Shanghai, China.
- **Poin Penting**:
  - XGBoost memperbaiki prediksi secara signifikan dibanding hanya mengandalkan model kimia-transport WRF-Chem saja.
  - Metode gabungan (*hybrid*) cuaca/numerik + ML menjadi terobosan sistem operasional peramalan cuaca lokal.

### 11. Air Quality Class Prediction Using ML Methods Based on Monitoring Data and Secondary Modeling
- **Fokus Utama**: Pemodelan sekunder menggunakan *Random Forest* untuk memprediksi kelas kualitas udara berbasis penggabungan observasi meteorologi dan proyeksi di Jinan, Tiongkok.
- **Poin Penting**:
  - Analisis signifikansi faktor meteorologi (suhu, kelembapan, tekanan udara) terhadap berbagai polutan menunjukkan korelasi yang sangat kuat secara musiman.

### 12. Air Quality Prediction and Ranking Assessment Based on Bootstrap-XGBoost Algorithm and Ordinal Classification Models
- **Fokus Utama**: Memprediksi angka AQI di Xi'an, Tiongkok (dengan XGBoost berbasis *Bootstrap*) serta klasifikasi peringkat kualitas udara dengan *Ordinal Logit/Probit regression*.
- **Poin Penting**:
  - Pendekatan 2-arah: Model pertama memberikan prediksi nilai kontinu (AQI beserta interval kepercayaannya), sedangkan model kedua khusus menebak kategori kelas (ranking).

### 13. Prediction of Air Quality Index Using Ensemble Models
- **Fokus Utama**: Memprediksi AQI di Kampung Kalipaten, Tangerang berbasis sensor IoT menggunakan keluarga *Ensemble Learning* (Bagging, RF, Gradient Boosting, AdaBoost).
- **Poin Penting**:
  - Model *Gradient Boosting Regressor* unggul tipis dibanding yang lain.
  - Bukti bahwa model *Ensemble* sangat kuat dalam meminimalisasi *bias* untuk data polusi sensor skala kampung/komunitas.

### 14. Machine Learning-Based Forecasting of Air Quality Index under Long-Term Environmental Patterns
- **Fokus Utama**: Perbandingan XGBoost, LightGBM, dan SVM pada data meteorologi dan polutan jangka panjang (8 tahun) di Türkiye Timur (2016-2024).
- **Poin Penting**:
  - XGBoost kembali terbukti menjadi algoritma dengan akurasi tertinggi untuk rentang data historis panjang dengan R² nyaris mendekati sempurna (0.999).

### 15. Machine Learning for Air Quality Prediction and Data Analysis: Review on Recent Advancements, Challenges, and Outlooks
- **Fokus Utama**: Sebuah *literature review* (makalah tinjauan) dari 78 studi tentang aplikasi *Machine Learning* untuk pemantauan kualitas udara.
- **Poin Penting**:
  - *Ensemble methods* (RF, XGBoost) unggul di dataset terstruktur (*tabular*).
  - *Deep learning* paling bagus untuk menangkap tren polusi spatio-temporal.
  - Tantangan masa depan adalah pada aspek *Explainability* (keterjelasan AI) dan implementasi *real-time* massal.

### 16. XGBoost: A Scalable Tree Boosting System
- **Fokus Utama**: Publikasi *original* sistem XGBoost (oleh Tianqi Chen) yang saat ini sangat luas digunakan untuk masalah data tabular termasuk kualitas udara.
- **Poin Penting**:
  - Memperkenalkan *sparsity-aware algorithm* dan pemrosesan komputasi *cache* yang cepat sehingga sanggup memproses triliunan sampel secara efisien.

### 17. Air Quality Forecasting Using Machine Learning: Comparative Analysis and Ensemble Strategies for Enhanced Prediction
- **Fokus Utama**: Menguji 10 model Machine Learning yang diterapkan pada Dataset Air Quality Kaggle (diambil dari sensor *metal oxide*), dilengkapi *Bayesian Optimization* dan *Stacking Ensemble*.
- **Poin Penting**:
  - Berbeda dengan jurnal lain, di sini SVR (*Support Vector Regression*) yang dioptimalkan dengan *Bayesian* menduduki peringkat pertama.
  - *Stacking* (menggabungkan kekuatan beberapa model dasar) sukses memetakan dinamika spatio-temporal tingkat tinggi.

### 18. Air Quality Prediction Models Based on Meteorological Factors and Real-Time Data of Industrial Waste Gas
- **Fokus Utama**: Model regresi *Random Forest* untuk distrik Zhangdian menggunakan input yang tidak lazim: data emisi pembuangan gas pabrik (*industrial waste gas*).
- **Poin Penting**:
  - Model dapat menghitung batas maksimun emisi harian limbah gas secara "terbalik" (inversi model) untuk memastikan udara tetap sehat di esok hari, menjembatani industri dan pelestarian lingkungan.

### 19. Using Machine Learning Algorithms to Study the Relationship Between Meteorological Conditions and Air Quality Parameters
- **Fokus Utama**: Meneliti hubungan non-linear kondisi meteorologi terhadap polutan di wilayah kering (*arid region*) Arab Saudi Timur.
- **Poin Penting**:
  - Gradient Boosting paling akurat memprediksi NO2 dengan mengaitkannya dengan faktor *kelembapan* dan *titik embun* (dew point).
  - Khusus PM10, akurasi sangat rendah lantaran PM10 di sana dipengaruhi badai pasir alam, bukan sekadar cuaca/aktivitas manusia.

### 20. Optimization of CNN-LSTM Air Quality Prediction Based on the POA Algorithm
- **Fokus Utama**: Model canggih *CNN-LSTM* di Changchun (China) yang fitur pentingnya diekstrak menggunakan *LightGBM* & *SHAP*, serta hyperparameter dioptimasi memakai *Pelican Optimization Algorithm (POA)*.
- **Poin Penting**:
  - POA terbukti mampu secara cerdas mencari struktur parameter CNN-LSTM yang memberi MAE terendah. Sangat andal untuk ketergantungan deret waktu durasi panjang.

### 21. Predicting the Concentration Levels of PM2.5 and O3 for Highly Urbanized Areas Based on ML Models
- **Fokus Utama**: Prediksi konsentrasi PM2.5 dan O3 di kawasan mega-urban Beijing-Tianjin-Hebei.
- **Poin Penting**:
  - Menemukan korelasi kuat antara PM10/CO dengan timbulnya PM2.5, serta korelasi antara suhu/NO2 dengan pembentukan O3.
  - Model XGBoost adalah alat *cost-effective* paling mumpuni untuk prediksi di wilayah ini.

### 22. Pengujian Algoritma Long Short Term Memory untuk Prediksi Kualitas Udara dan Suhu Kota Bandung
- **Fokus Utama**: Memprediksi data *time-series* PM10, ISPU, suhu, dan kelembapan kota Bandung dengan 4 *hidden layer* LSTM.
- **Poin Penting**:
  - Secara berurutan, prediksi terbaik dicapai pada variabel kelembapan, suhu, dan ISPU, namun memiliki error yang agak tinggi pada variabel PM10.

### 23. Analisis dan Prediksi Indeks Kualitas Udara Jakarta: Penerapan Algoritma XGBoost
- **Fokus Utama**: Mengumpulkan prediktor AQI kota Jakarta melalui *data mining* citra satelit (*Earth Engine Code Editor*) lalu dimodelkan dengan XGBoost.
- **Poin Penting**:
  - Feature Importance Analysis menemukan bahwa *SO2*, *PM2.5*, dan *PM10* adalah "biang kerok" utama perburukan kualitas udara Jakarta.

### 24. Prediksi Kualitas Udara Malang Menggunakan Metode Gradient Boosting Regression
- **Fokus Utama**: Memprediksi lonjakan status "Tidak Sehat" untuk kualitas udara kota Malang, yang sepanjang tahun 2023 terjadi hingga 47 kali.
- **Poin Penting**:
  - Model *Gradient Boosting Regression* terintegrasi antarmuka interaktif *Streamlit*. Model memproyeksikan hari-hari ke depan yang diprediksi jatuh pada level "Tidak Sehat" untuk peringatan dini.

---
*Dibuat oleh AI Assistant untuk menyarikan koleksi jurnal Vany Salsabila Putri.*
