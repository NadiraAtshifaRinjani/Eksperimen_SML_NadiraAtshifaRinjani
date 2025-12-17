# Eksperimen_SML_NadiraAtshifaRinjani

Repository ini dibuat untuk memenuhi **Kriteria 1 – Melakukan Eksperimen terhadap Dataset Pelatihan**

Proyek ini mencakup proses eksplorasi data, preprocessing manual melalui notebook, serta otomatisasi preprocessing menggunakan Python script dan GitHub Actions.

## Struktur Repository

Eksperimen_SML_NadiraAtshifaRinjani
├── .github/workflows
│ └── preprocessing.yml
├── dataset_raw
│ └── datarumah.csv
├── preprocessing
│ ├── Eksperimen_Nadira_Atshifa_Rinjani.ipynb
│ ├── automate_NadiraAtshifaRinjani.py
│ └── datasetumah_preprocessing
│ └── data_preprocessed.csv
└── README.md

## Dataset

Dataset yang digunakan merupakan data rumah yang berisi informasi seperti harga rumah, luas bangunan dan tanah, jumlah kamar tidur dan kamar mandi, kondisi rumah, jumlah lantai, dan fitur lainnya. Dataset mentah disimpan pada folder `dataset_raw`.

## Eksperimen & Preprocessing

Proses eksplorasi dan preprocessing data dilakukan secara manual pada notebook:
"preprocessing/Eksperimen_Nadira_Atshifa_Rinjani.ipynb"

Tahapan yang dilakukan meliputi data loading, exploratory data analysis (EDA), penanganan outlier, transformasi log, encoding fitur kategorikal, dan feature scaling

## Automasi Preprocessing

Automasi preprocessing dilakukan menggunakan script Python berikut:
"preprocessing/automate_NadiraAtshifaRinjani.py"

Script ini membaca dataset mentah, menerapkan seluruh tahapan preprocessing hasil eksperimen, dan menyimpan dataset hasil preprocessing dalam format CSV pada folder `preprocessing/datasetumah_preprocessing`.


## GitHub Actions

Repository ini menggunakan GitHub Actions untuk menjalankan preprocessing secara otomatis. Workflow berada pada:
".github/workflows/preprocessing.yml"

Workflow akan berjalan ketika terjadi push ke branch `main` atau dijalankan secara manual. Hasil preprocessing akan disimpan sebagai **artifact** dengan nama:
"preprocessed-dataset"

Artifact ini dapat diunduh melalui tab **Actions** pada repository.


## Author

**Nadira Atshifa Rinjani**
