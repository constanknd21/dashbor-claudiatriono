# 🤖 Dashboard Analisis Sentimen PSU (Pemilihan Suara Ulang)

Dashboard interaktif berbasis **Streamlit** untuk menganalisis opini publik terhadap Pemilihan Suara Ulang (PSU) di media sosial X (Twitter), menggunakan model **CNN (Convolutional Neural Networks)**.

---

## 📊 Fitur Dashboard

| Tab | Fitur |
|---|---|
| 📊 Ringkasan Eksekutif | KPI metrik, pie chart komposisi sentimen, tren sentimen harian |
| ☁️ Analisis Teks | Word Cloud per kategori sentimen, distribusi panjang teks |
| 🎯 Evaluasi Model CNN | Confusion Matrix, Classification Report, akurasi 92.20% |
| 🔎 Filter & Ekspor | Filter data interaktif, pencarian kata kunci, download CSV |

---

## 📁 Struktur File

```
analisis_psu/
├── app.py                      # Aplikasi Streamlit utama
├── data_psu.csv                # Dataset utama (1.016 tweet, sudah berlabel)
├── pemilihan_suara_ulang.csv   # Dataset mentah hasil scraping X (Twitter)
├── requirements.txt            # Dependensi Python
└── README.md                   # Dokumentasi proyek
```

---

## 📦 Dataset

- **Sumber:** X (Twitter) — scraping dengan kata kunci PSU / Pemilihan Suara Ulang
- **Total Data:** 1.016 tweet (setelah preprocessing)
- **Distribusi Sentimen:**
  - Netral: 807 tweet (79.4%)
  - Positif: 186 tweet (18.3%)
  - Negatif: 23 tweet (2.3%)
- **Metode Pelabelan:** Kombinasi Leksikon + Validasi Manual

---

## 🚀 Cara Menjalankan Lokal

**1. Clone repository**
```bash
git clone https://github.com/username/analisis_psu.git
cd analisis_psu
```

**2. Install dependensi**
```bash
pip install -r requirements.txt
```

**3. Jalankan aplikasi**
```bash
streamlit run app.py
```

---

## 🌐 Deploy di Streamlit Cloud

1. Push repo ini ke GitHub
2. Buka [share.streamlit.io](https://share.streamlit.io)
3. Klik **New app** → pilih repo ini
4. Set **Main file path:** `app.py`
5. Klik **Deploy**

---

## 🧰 Tech Stack

- **Frontend:** Streamlit 1.28.1
- **Data Processing:** Pandas 2.0.3
- **Visualisasi:** Plotly 5.20.0, Matplotlib 3.7.2
- **NLP:** WordCloud 1.9.3
- **Model:** CNN (Convolutional Neural Networks)

---

## 👨‍💻 Tentang Proyek

Proyek ini merupakan penelitian analisis sentimen terhadap wacana Pemilihan Suara Ulang (PSU) di Indonesia menggunakan pendekatan deep learning berbasis CNN.
