Muhammad Farhan

Fasya Burhanis Syauqi

# 🎭 GoEmotions: Multi-Label Emotion Classification

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-2.0%2B-orange)
![HuggingFace](https://img.shields.io/badge/Transformers-4.30%2B-yellow)
![Task](https://img.shields.io/badge/Task-Multi--Label-red)

Proyek ini mengimplementasikan model **Multi-Label Classification** menggunakan **DistilBERT** untuk mendeteksi emosi kompleks dalam teks. Berbeda dengan klasifikasi standar, model ini mampu memprediksi **lebih dari satu emosi** sekaligus untuk satu kalimat input.

## 📌 Tentang Dataset
Dataset yang digunakan adalah **GoEmotions (Simplified)** yang dirilis oleh Google Research.
- **Total Label:** 28 Kategori Emosi (termasuk *Neutral*).
- **Tipe:** Multi-label (Satu teks bisa memiliki label [0, 1, 0, ..., 1]).
- **Contoh Label:** `Admiration`, `Amusement`, `Anger`, `Joy`, `Fear`, `Surprise`, dll.

## 📂 Struktur Proyek
```text
project_goemotions/
├── notebooks/
│   └── Task2_GoEmotions.ipynb   # Notebook Training & Fix Error Handling
├── reports/
│   └── report.md                # Laporan analisis F1-Score
├── requirements.txt             # Dependencies
└── README.md                    # Dokumentasi
