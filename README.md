# 🏡 Airbnb Listings in Bangkok - Analysis and Recommendations

## 📌 Business Overview

Pasar Airbnb di Bangkok merupakan salah satu yang paling aktif di Asia Tenggara, menarik wisatawan dari seluruh dunia. Namun, dengan persaingan listing yang tinggi dan preferensi tamu yang beragam, pemilik properti perlu memahami tren pasar, preferensi lokasi, dan strategi harga untuk memaksimalkan profit.

Proyek ini bertujuan membantu pemilik atau calon pemilik properti di Bangkok membuat keputusan berbasis data yang lebih baik terkait lokasi, jenis akomodasi, dan segmentasi harga.

## 🎯 Goal Statement

Menyediakan insight dan rekomendasi data-driven terkait:

- Area (neighbourhood) yang potensial untuk listing baru
- Tipe akomodasi yang paling diminati dan menguntungkan
- Segmentasi harga berdasarkan pasar aktual untuk membantu strategi penetapan harga

## 📐 Scope of Metrics

Beberapa metrik utama yang dianalisis dalam proyek ini meliputi:

- **Price**: Distribusi harga listing dan segmentasinya
- **Neighbourhood performance**: Berdasarkan rata-rata harga, jumlah review, dan tingkat ketersediaan
- **Room type preference**: Analisis popularitas dan performa berdasarkan jenis ruangan
- **Reviews data**: Indikator permintaan dan reputasi listing

## 📊 Analisis yang Dilakukan

### 1. Neighbourhood Recommendation
- Evaluasi performa area berdasarkan harga, jumlah review, dan availability.
- Rekomendasi lokasi potensial untuk listing baru.

### 2. Room Type Recommendation
- Analisis tren dan performa tiap tipe ruangan.
- Identifikasi jenis akomodasi dengan revenue potensial tertinggi.

### 3. Price Segmentation
- Clustering harga untuk mengelompokkan listing ke dalam segmen low-end, mid-range, dan high-end.
- Memberikan strategi penetapan harga sesuai dengan target pasar.

## 📈 Interactive Dashboard

Lihat visualisasi interaktif proyek ini di Tableau Public:  
🔗 [Tableau Dashboard – Airbnb Bangkok](https://public.tableau.com/app/profile/abednego.andries/viz/Airbnb_Visualization_17442052583890/Aboutus)

## 📁 Dataset Description

### Filename: `Airbnb Listings Bangkok Clean.csv`

| Column Name                   | Data Type  | Description |
|--------------------------------|-----------|-------------|
| `id`                          | Object    | Airbnb's unique identifier for the listing. |
| `name`                        | Object    | Name of the listing. |
| `host_id`                     | Object    | Airbnb's unique identifier for the host/user. |
| `host_name`                   | Object    | Name of the host (usually first name). |
| `neighbourhood`               | Category  | Geocoded neighborhood based on latitude and longitude. |
| `latitude`                    | Float     | Latitude coordinate (WGS84 projection). |
| `longitude`                   | Float     | Longitude coordinate (WGS84 projection). |
| `room_type`                   | Category    | Type of room: Entire home/apt, Private room, Shared room, or Hotel. |
| `price`                       | Float     | Daily price in local currency. |
| `minimum_nights`              | Integer   | Minimum number of nights required for booking. |
| `number_of_reviews`           | Integer   | Total number of reviews received. |
| `last_review`                 | DateTime  | Date of the most recent review. |
| `reviews_per_month`           | Float  | Average reviews per month. |
| `calculated_host_listings_count` | Integer   | Number of listings the host has in the current region. |
| `availability_365`            | Integer   | Number of days the listing is available in a year. Note: a listing may be unavailable because it has been booked by a guest or blocked by the host.|
| `number_of_reviews_ltm`       | Integer   | Number of reviews received in the last 12 months. |
| `recency`       | Integer   | Number of days since listing receive reviews from last review dates. |
| `revenue_at_least`       | Integer   | Number of revenue received by hosts based on `price` x `minimum_nights` x `number_of_reviews` |
| `empty_listing`       | Integer   | Identifier for listings which have 0 `number_of_reviews` (1) and listings which have more than 0 `number_of_reviews`. |

## 🔧 Tools & Libraries

- Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn)
- Jupyter Notebook (`Airbnb_Analytics.ipynb`)
- Tableau Public
- GitHub

## 🚀 How to Use

1. Clone repo ini:
   ```bash
   git clone https://github.com/username/airbnb-bangkok-analysis.git
   cd airbnb-bangkok-analysis
   ```

2. Buka file `Airbnb_Analytics.ipynb` di Jupyter Notebook dan mulai eksplorasi.

3. Kunjungi dashboard Tableau untuk insight visual.
