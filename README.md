# 🚀 Prediksi Keterlambatan Pengiriman - FESMARO 2025 📦

### **Tim PNJoy**
- **Syifa Azzahirah** - 2207411024  
- **Deva Alvyn Budinugraha** - 2207411050  
- **Nabil Falih Khairullah** - 2107411060  

📍 **Politeknik Negeri Jakarta**  
📅 **Kompetisi: Analisis Big Data - FESMARO 2025**

---

## 📌 Deskripsi Proyek
Dalam industri **Supply Chain Management**, keterlambatan pengiriman dapat menyebabkan **penurunan kepuasan pelanggan dan peningkatan biaya operasional**. Oleh karena itu, proyek ini bertujuan untuk **memprediksi keterlambatan pengiriman berdasarkan data historis transaksi** menggunakan **Machine Learning (Random Forest & XGBoost).**  

### 🔍 Fokus Analisis
✅ **Mengidentifikasi faktor utama** yang mempengaruhi keterlambatan pengiriman.  
✅ **Membangun model prediksi keterlambatan** dengan Machine Learning.  
✅ **Menganalisis performa model** dengan berbagai metrik evaluasi.  

---

## 📊 Dataset
Dataset yang digunakan adalah **DataCo Smart Supply Chain** yang berisi informasi transaksi dan logistik dengan lebih dari **180.000 transaksi**.  

**Fitur utama yang digunakan:**
- **Tanggal Pemesanan & Pengiriman** 📅 (`order date`, `Days for shipping (real)`)
- **Kategori Produk** 🏷️ (`Category Name`)
- **Lokasi Pengiriman** 📍 (`Customer City`, `Order Region`)
- **Mode Pengiriman** 🚚 (`Shipping Mode`)

---

## 📖 Metodologi
### 1️⃣ Data Preparation
✔ **Menghapus missing values & duplikasi**.
✔ **Encoding fitur kategorikal dengan One-Hot Encoding**.
✔ **Normalisasi fitur numerik dengan StandardScaler**.

### 2️⃣ Feature Engineering
✔ **Membuat fitur baru `Shipment_Delay`** sebagai selisih waktu pengiriman real vs jadwal.  
✔ **Ekstraksi fitur waktu (Order Year, Month, Day) untuk analisis pola musiman.**  

### 3️⃣ Model Training & Evaluation
🔹 **Model yang digunakan:**
- **Random Forest** 🌲  
- **XGBoost** 🚀  

🔹 **Metrik Evaluasi:**
📌 **Accuracy, Precision, Recall, F1-Score, Confusion Matrix, ROC-AUC Curve.**  

---

## 📊 Hasil Evaluasi
| Model          | Accuracy | Precision | Recall | F1-Score | AUC-ROC |
|---------------|----------|-----------|--------|----------|---------|
| Random Forest | **81.49%** | 81.00%       | 81.00%    | 81.00%      | **0.88** |
| XGBoost       | 71.71%   | 76.00%       | 74.00%    | 72.00%      | 0.78    |

📢 **Kesimpulan:**  
🎯 **Random Forest adalah model terbaik** dengan akurasi **81.49%** dan AUC **0.88**.  

---

## 📁 File dalam Repository

### 📌 **1. Model Terlatih**
- **`random_forest_best.pkl`** → Model Machine Learning yang sudah dilatih menggunakan **Random Forest**.
- Digunakan untuk **memprediksi keterlambatan pengiriman** berdasarkan data input yang telah diproses.

### 📌 **2. Dataset yang Telah Diproses**
- **`FF_processed_dataset.csv`** → Dataset hasil **preprocessing dan feature engineering**.
- Berisi fitur-fitur yang telah diolah untuk digunakan dalam training model.

---

## 📌 Cara Menjalankan Kode
### 1️⃣ Clone Repository
```bash
git clone https://github.com/Seismiks/Fesmaro-DataCo.git
cd Fesmaro-DataCo
```

### 2️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 3️⃣ Jalankan Notebook di Google Colab
- **Link Google Colab:** [Klik di sini](https://colab.research.google.com/drive/1BmgbY87BSnczjrPju67ZqWENbD7sw2za#scrollTo=rRl3aGqcuxJZ)
- **Jalankan semua cell** untuk preprocessing, training, dan evaluasi model.

---

## 📌 Struktur Repository
```
📂 FESMARO_2025_Supply_Chain_Prediction
│── 📜 README.md          <- Dokumentasi proyek ini
│── 📂 src                <- Kode sumber (Preprocessing & Training Model)
│── 📂 data               <- Dataset yang digunakan
│── 📂 reports            <- Laporan PDF & hasil analisis
│── 📂 notebooks          <- Jupyter Notebook / Google Colab eksperimen
│── 📂 models             <- Model yang sudah dilatih (Saved Models)
```

---

## 🔗 Link Pengumpulan
📌 **GitHub Repository:** [https://github.com/Seismiks/Fesmaro-DataCo](https://github.com/Seismiks/Fesmaro-DataCo)  
📌 **Google Colab Notebook:** [https://colab.research.google.com/drive/1BmgbY87BSnczjrPju67ZqWENbD7sw2za#scrollTo=rRl3aGqcuxJZ](https://colab.research.google.com/drive/1BmgbY87BSnczjrPju67ZqWENbD7sw2za#scrollTo=rRl3aGqcuxJZ)  

---

## 💡 Rekomendasi Pengembangan
🚀 **Tingkatkan akurasi model** dengan Hyperparameter Tuning (GridSearchCV).  
🚀 **Tambahkan faktor eksternal** (cuaca, lalu lintas, hari libur) untuk model lebih akurat.  
🚀 **Integrasikan model ini ke dalam dashboard** untuk mempermudah pemantauan pengiriman.  


---

🎯 **Tim PNJoy - Politeknik Negeri Jakarta**  
🏆 **FESMARO 2025 - Analisis Big Data**  

🔥 **Ayo tingkatkan efisiensi rantai pasok dengan Machine Learning!** 🚀  

---
