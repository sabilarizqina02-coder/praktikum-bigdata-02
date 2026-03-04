

# README.md

```markdown
# Big Data Technology Practicum 02
## Batch Data Ingestion & Processing with Apache Spark

Praktikum ini bertujuan untuk mengimplementasikan pipeline pemrosesan data batch menggunakan Apache Spark. Pipeline ini melakukan proses ingestion, cleaning, transformasi, dan analisis data e-commerce.

Melalui praktikum ini mahasiswa memahami konsep dasar data engineering seperti batch processing, data cleaning, agregasi data, serta penyimpanan data menggunakan format yang lebih efisien.

---

# Dataset

Dataset yang digunakan adalah dataset transaksi e-commerce yang tersimpan dalam format CSV.

Lokasi dataset:

data/raw/ecommerce_raw.csv

Dataset ini berisi informasi transaksi seperti:

- Product
- Category
- Quantity
- Price
- Timestamp

---

# Struktur Folder Project

Struktur folder project yang digunakan adalah sebagai berikut:

```

bigdata-project/
│
├── data/
│   ├── raw/
│   │   └── ecommerce_raw.csv
│   │
│   ├── clean/
│   │   ├── parquet/
│   │   └── partitioned_by_category/
│   │
│   └── curated/
│       ├── avg_transaction/
│       ├── category_revenue/
│       └── top_products/
│
├── logs/
│   └── batch_pipeline.log
│
├── scripts/
│   └── batch_pipeline_enterprise.py
│
└── README.md

```

---

# Teknologi yang Digunakan

Teknologi yang digunakan dalam praktikum ini antara lain:

- Python
- Apache Spark (PySpark)
- Linux Environment (WSL)
- VS Code
- Parquet File Format

---

# Setup Environment

Aktifkan virtual environment terlebih dahulu sebelum menjalankan pipeline:

```

source venv/bin/activate

```

---

# Menjalankan Pipeline

Untuk menjalankan pipeline data processing gunakan perintah berikut:

```

python scripts/batch_pipeline_enterprise.py

```

Pipeline akan melakukan beberapa tahapan:

1. Inisialisasi Spark Session
2. Load dataset dari CSV
3. Data cleaning
4. Transformasi data
5. Perhitungan business metrics
6. Menyimpan hasil ke format Parquet

---

# Output Pipeline

Pipeline akan menghasilkan beberapa output analisis:

### 1. Total Raw Records
Menampilkan jumlah data mentah yang dimuat dari dataset.

### 2. Total Cleaned Records
Menampilkan jumlah data setelah proses pembersihan.

### 3. Top 5 Products
Menampilkan 5 produk dengan jumlah penjualan tertinggi.

### 4. Category Revenue
Menampilkan total pendapatan berdasarkan kategori produk.

### 5. Clean Data (Parquet)
Data yang telah dibersihkan disimpan dalam format Parquet agar lebih efisien.

---

# Hasil Eksekusi

Jika pipeline berhasil dijalankan maka terminal akan menampilkan:

```

PIPELINE COMPLETED SUCCESSFULLY

```

Selain itu juga akan ditampilkan waktu eksekusi pipeline.

---

# Kesimpulan

Dari praktikum ini dapat dipahami proses dasar dalam data engineering menggunakan Apache Spark. Pipeline yang dibuat mampu melakukan ingestion, pembersihan data, transformasi, serta analisis data secara efisien menggunakan format penyimpanan Parquet.

---

# Author

Nama: Sabila Rizqina Majid  
Program Studi: Teknologi Informasi  
Universitas: UIN Antasari
```

