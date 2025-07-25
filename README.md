# Sentiment Analysis with IndoBERT + Flask

Sebuah aplikasi analisis sentimen sederhana berbasis teks bahasa Indonesia menggunakan model IndoBERT dan disajikan melalui web dengan Flask.

## 🚀 Fitur

- Model analisis sentimen berbasis IndoBERT
- Web interface menggunakan Flask
- Prediksi sentimen positif/negatif terhadap input teks
- Training model menggunakan dataset kustom

## 📂 Struktur Folder

ai-ml/
│
├── app.py # Web server Flask
├── model/
│ ├── train.py # Script untuk training model
│ ├── predict.py # Script prediksi menggunakan model
│ └── (tf_model.h5) # File model hasil training (tidak diunggah ke GitHub)
│
├── templates/
│ └── index.html # UI web
├── dataset.csv # Dataset training
├── requirements.txt # Daftar library Python
└── README.md # Dokumentasi ini


## 🧠 Cara Training Model

1. Pastikan kamu punya `dataset.csv` dengan format:
    ```
    text,label
    "Saya senang dengan layanan ini",1
    "Pelayanannya buruk",0
    ```

2. Jalankan training:

```bash
cd model
python train.py

pip install -r requirements.txt

python app.py

Buka browser dan akses: http://localhost:5000
