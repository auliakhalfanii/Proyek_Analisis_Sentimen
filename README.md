# Analisis Sentimen Ulasan Aplikasi Shopee

## 📌 Deskripsi Proyek

Proyek ini bertujuan untuk menganalisis **sentimen dari 10.000 ulasan pengguna aplikasi Shopee** yang diambil dari Google Play Store. Dengan menerapkan teknik pra-pemrosesan teks dan algoritma machine learning, proyek ini mengklasifikasikan ulasan menjadi tiga kategori: **positif**, **negatif**, dan **netral**.

---

## 🗂️ Tahapan Proyek

1. **Scraping & Pembersihan Data**
   - Data diambil dari aplikasi `com.shopee.id`.
   - Total data awal: 10.000 ulasan.
   - Setelah pembersihan dan penghapusan duplikat: ±11.991 ulasan.

2. **Preprocessing Teks**
   - Case folding (lowercase)
   - Normalisasi kata tidak baku (slangword)
   - Tokenisasi
   - Stopword removal
   - Stemming (menggunakan Sastrawi)
   - Hasil akhir disimpan 

3. **Pelabelan Sentimen (Lexicon-Based)**
   - Berdasarkan jumlah kata positif dan negatif.
   - Label

4. **Eksplorasi Data & WordCloud**
   - Distribusi jumlah ulasan per kategori sentimen.
   - WordCloud untuk tiap kategori sentimen.

5. **Ekstraksi Fitur**
   - Menggunakan **TF-IDF Vectorizer** untuk merepresentasikan teks.

6. **Pelatihan Model**
   - **Random Forest** + TF-IDF + Cross Validation
   - **SVM (Support Vector Machine)** + SMOTE untuk menangani imbalance data
   - **Feature Selection** untuk meningkatkan performa

7. **Evaluasi Model**
   - Metode evaluasi:
     - Accuracy
     - Confusion Matrix
     - Cross Validation Score
   - Perbandingan performa antar model divisualisasikan

---

## 🛠 Teknologi dan Library

- Python 3.x
- Jupyter Notebook
- `pandas`, `numpy` – manipulasi data
- `scikit-learn` – machine learning
- `Sastrawi`, `nltk` – preprocessing teks
- `matplotlib`, `seaborn`, `wordcloud` – visualisasi
- `imblearn` – SMOTE untuk penyeimbangan kelas

---

## 📈 Hasil

Model **Random Forest** dan **SVM** menunjukkan akurasi yang kompetitif dalam mengklasifikasikan ulasan. Feature selection dan SMOTE memberikan dampak positif terhadap performa akhir model.

---

## 👩‍💻 Kontributor

- Aulia Khalfani Izzati Kurdiana

---

## 📄 Lisensi

Proyek ini dibuat untuk keperluan edukasi dan penelitian.
