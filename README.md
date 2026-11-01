# Olist E-Commerce Customer Segmentation (RFM & K-Means)

## 📌 Deskripsi Proyek
Proyek ini merupakan analisis data *end-to-end* menggunakan dataset publik Olist, platform e-commerce di Brasil. Tujuan utama proyek ini adalah melakukan pembersihan data (*Data Engineering*), *Exploratory Data Analysis* (EDA), dan membangun segmentasi pelanggan untuk merumuskan strategi retensi bisnis.

## 🛠️ Metodologi & Teknologi
* **Bahasa & Library:** Python, Pandas, Matplotlib, Seaborn, Scikit-Learn.
* **Data Engineering:** Penggabungan berbagai tabel relasional (Orders, Products, Customers, Payments, dll), penanganan *missing values*, dan transformasi tipe data.
* **Analisis RFM:** Mengelompokkan pelanggan berdasarkan *Recency* (Keterbaruan), *Frequency* (Frekuensi), dan *Monetary* (Nilai Moneter).
* **Machine Learning:** Menerapkan algoritma **K-Means Clustering** (dioptimasi dengan *Elbow Method*) untuk mengidentifikasi kelompok pelanggan secara otomatis.

## 📊 Temuan Bisnis Utama
Berdasarkan hasil K-Means Clustering dengan nilai *k=4*, pelanggan terbagi ke dalam 4 segmen:
1. **Lost Cheap Customers (Mayoritas):** Pelanggan yang hanya berbelanja sekali dengan nilai transaksi rendah dan sudah lama tidak kembali.
2. **Lost Big Spenders:** Mantan VIP yang menghabiskan banyak uang di masa lalu namun sudah lama tidak aktif.
3. **Recent / New Customers:** Pelanggan yang baru saja melakukan transaksi pertama mereka.
4. **Loyal Customers (Minoritas):** Kelompok terkecil namun paling berharga yang berbelanja lebih dari satu kali dengan nilai transaksi tinggi.

**Rekomendasi Strategis:** Olist memiliki tingkat akuisisi yang baik namun tingkat retensi pelanggan (*customer retention*) yang rendah. Anggaran pemasaran sebaiknya difokuskan pada kampanye *follow-up* (seperti diskon pembelian kedua atau program loyalitas) yang ditargetkan pada "Recent/New Customers" untuk mencegah mereka beralih menjadi "Lost Customers".

## 🚀 Cara Menjalankan Proyek
1. Clone repositori ini: `git clone [[URL_REPOSITORI_ANDA]](https://github.com/al-DataEngineer/olist-ecommerce-segmentation)`
2. Buka file `olist_customer_segmentation_rfm_kmeans.ipynb` menggunakan Jupyter Notebook atau VS Code.
3. Pastikan mengunduh raw dataset dari Kaggle (Olist Store) jika ingin mengeksekusi ulang keseluruhan skrip.
