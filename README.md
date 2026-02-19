# 🧠 Analisis Risiko Stroke & Segmentasi Pasien

## 📌 Project Overview

Stroke merupakan salah satu penyebab kematian dan disabilitas tertinggi secara global.  
Project ini bertujuan untuk menganalisis faktor-faktor yang berkontribusi terhadap kejadian stroke serta mengidentifikasi kelompok pasien dengan risiko tertinggi berdasarkan data pasien.

Analisis dilakukan menggunakan pendekatan Exploratory Data Analysis (EDA) dan segmentasi risiko untuk menghasilkan insight yang dapat mendukung strategi pencegahan dini.

---

## 🎯 Tujuan Bisnis

Project ini bertujuan untuk membantu institusi kesehatan dalam:

- Mengidentifikasi faktor risiko utama stroke  
- Menentukan kelompok pasien berisiko tinggi  
- Mendukung strategi screening dan pencegahan berbasis data  

---

## 📊 Informasi Dataset

- Sumber: Kaggle – Stroke Prediction Dataset  
- Total Data: 4.860 pasien  
- Target Variabel: `stroke`  
  - 1 = Stroke  
  - 0 = Tidak Stroke  

### Variabel Utama:

- Age  
- Gender  
- Hypertension  
- Heart Disease  
- Avg Glucose Level  
- BMI  
- Smoking Status  
- Residence Type  
- Work Type  

---

## 🧹 Data Preparation

Langkah-langkah yang dilakukan:

- Pengecekan missing value dan data duplikat
- Terdapat missing value dan untuk handlingnya dengan imputasi BMI menggunakan nilai median 
- Validasi outlier pada Age, BMI, dan Glucose. Setelah dilakukan pengecekan outlier tidak dihapus karena masih berada dalam rentang medis yang realistis.
- Transformasi variabel numerik menjadi kategori:
  - Age → Age Category  
  - BMI → BMI Category  
  - Avg Glucose → Glucose Category  
- Pembuatan variabel kombinasi risiko (Hipertensi + Penyakit Jantung)


---

## 📊 Exploratory Data Analysis (EDA)

EDA dilakukan dalam tiga tahap:

### 1️⃣ Univariate Analysis  
Memahami distribusi usia, BMI, kadar glukosa, dan proporsi stroke.

### 2️⃣ Bivariate Analysis  
Menganalisis hubungan antara stroke dengan:
- Usia  
- Hipertensi  
- Penyakit jantung  
- BMI  
- Glukosa  

### 3️⃣ Multivariate & Segmentasi Risiko  
- Heatmap interaksi usia dan komorbid  
- Analisis kombinasi risiko  
- Identifikasi faktor dominan  

---

## 🔎 Insight Utama

- Usia merupakan faktor risiko paling dominan terhadap stroke  
- Penyakit jantung dan hipertensi meningkatkan risiko secara signifikan  
- Kombinasi hipertensi dan penyakit jantung menunjukkan risiko tertinggi  
- Kadar glukosa tinggi berkorelasi dengan peningkatan risiko stroke  
- BMI overweight/obese dan riwayat merokok memperkuat risiko  
- Kasus stroke lebih banyak ditemukan pada populasi urban  

---

## 🏥 Rekomendasi

- Prioritaskan screening untuk pasien usia di atas 50 tahun  
- Monitoring intensif pasien dengan penyakit kronis  
- Dorong kontrol gula darah secara rutin  
- Tingkatkan edukasi pola hidup sehat  
- Perkuat program pencegahan di wilayah urban  

---

## 🛠 Tools yang Digunakan

- Python (Pandas, Matplotlib, Seaborn)  
- Tableau (Dashboard Interaktif)  
- Jupyter Notebook  

---

