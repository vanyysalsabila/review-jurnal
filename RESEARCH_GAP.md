# 🔍 Analisis Research Gap (Celah Penelitian)

Berdasarkan tinjauan terhadap 24 jurnal penelitian mengenai **Prediksi Kualitas Udara (AQI) Menggunakan Machine Learning**, berikut adalah kompilasi *Research Gap* (celah penelitian) yang masih menjadi tantangan dan peluang untuk riset di masa depan:

## 1. Generalisasi Geografis (Geographical Generalizability)
* **Kondisi Saat Ini**: Mayoritas model dilatih dan diuji pada dataset lokal yang spesifik untuk satu kota atau wilayah tertentu (misal: hanya di Jakarta, Bandung, atau Beijing).
* **Research Gap**: Model yang sangat akurat di satu kota seringkali gagal atau menurun drastis performanya jika diterapkan di kota lain karena perbedaan topografi, iklim, dan sumber emisi. Dibutuhkan model hibrida atau pendekatan *Transfer Learning* (seperti pada jurnal ke-4) yang mampu menggeneralisasi prediksi dari wilayah kaya data ke wilayah yang minim stasiun pemantauan (*low-resource settings*).

## 2. Masalah "Black Box" dan Keterjelasan (Explainable AI / XAI)
* **Kondisi Saat Ini**: Algoritma dengan akurasi tertinggi seperti XGBoost, Random Forest, dan CNN-LSTM beroperasi layaknya "kotak hitam" (black-box).
* **Research Gap**: Pembuat kebijakan pemerintah membutuhkan alasan mengapa suatu prediksi dibuat (misal: "Mengapa esok hari diprediksi PM2.5 akan naik drastis?"). Masih sangat sedikit penelitian yang secara mendalam mengintegrasikan *Explainable AI* (seperti algoritma SHAP atau LIME) untuk memberikan interpretasi *feature importance* secara dinamis dan transparan.

## 3. Integrasi Data Spatio-Temporal Skala Besar
* **Kondisi Saat Ini**: Banyak studi hanya menggunakan satu atau dua jenis data (misal: data polutan historis + data suhu/kelembapan dasar).
* **Research Gap**: Terdapat celah untuk menggabungkan lebih banyak dimensi data secara *real-time*, seperti pergerakan lalu lintas (*traffic*), data citra satelit (AOD), ketinggian muka tanah, arah/kecepatan angin tiga dimensi, dan data emisi industri harian (seperti pada jurnal ke-18). Penggabungan ini membutuhkan arsitektur model *Deep Learning* yang lebih kompleks namun efisien.

## 4. Keakuratan Prediksi Jangka Panjang & Kondisi Ekstrem
* **Kondisi Saat Ini**: Model *Machine Learning* saat ini sangat andal untuk melakukan peramalan jangka pendek (1 hingga 48 jam ke depan).
* **Research Gap**: Akurasi peramalan jatuh secara signifikan untuk peramalan jangka panjang (mingguan/bulanan) dan sangat rentan terhadap kejadian anomali mendadak (seperti kebakaran hutan tiba-tiba, badai debu di Timur Tengah, atau lonjakan emisi libur panjang). Dibutuhkan algoritma yang lebih *robust* untuk menangani *outlier* dan kejadian ekstrem.

## 5. Keseimbangan Komputasi dan Penerapan pada Edge/IoT
* **Kondisi Saat Ini**: Untuk mencapai akurasi tinggi, peneliti berlomba-lomba menggunakan *Ensemble Models* yang tebal atau arsitektur Deep Learning (*Transformers / CNN-LSTM*) yang memakan resource komputasi besar.
* **Research Gap**: Bagaimana men-deploy model-model berat tersebut ke dalam infrastruktur sensor IoT yang memiliki daya dan memori terbatas (*Edge Computing*) masih menjadi tantangan. Model perlu di-kompresi (*model pruning* atau *quantization*) tanpa mengorbankan terlalu banyak akurasi.

## 6. Kekurangan Fokus pada Polutan Minor
* **Kondisi Saat Ini**: 90% penelitian berpusat pada PM2.5, PM10, dan O3 karena polutan ini paling berdampak pada kesehatan dan datanya paling mudah didapat.
* **Research Gap**: Polutan spesifik industri dan VOCs (*Volatile Organic Compounds*) sering diabaikan karena sulitnya pemantauan. Memasukkan elemen ini sangat penting bagi daerah yang berdampingan erat dengan kawasan industri berat.

---
### 💡 Kesimpulan untuk Topik Skripsi/Penelitian Lanjutan
Jika Anda ingin menyusun penelitian baru, Anda bisa "menyerang" celah-celah di atas. Misalnya:
> *"Penerapan Explainable AI (SHAP) pada algoritma XGBoost untuk memprediksi Indeks Kualitas Udara secara Real-Time dengan mengintegrasikan data Cuaca dan Lalu Lintas"*
