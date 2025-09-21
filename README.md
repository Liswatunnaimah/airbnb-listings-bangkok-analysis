# Airbnb Listings Bangkok Analysis

## Ringkasan Proyek
Proyek ini bertujuan untuk menganalisis data listing Airbnb di Bangkok guna mengidentifikasi karakteristik yang memengaruhi popularitas suatu listing. Analisis dilakukan untuk menjawab pertanyaan bisnis mengenai faktor apa saja yang meningkatkan visibilitas, jumlah pemesanan, dan ulasan, serta memberikan rekomendasi strategis baik bagi host maupun manajemen Airbnb.

---

## Dataset
- Sumber: Inside Airbnb (Bangkok snapshot)  
- Jumlah data: 15.845 listing, 6.651 host unik, mencakup 50 distrik  
- Periode: ulasan dari tahun 2012 hingga 2022  
- Variabel utama: tipe kamar, harga, jumlah minimum malam, ketersediaan, jumlah ulasan  
- Data Dictionary: [airbnb_data_dictionary.pdf](data/metadata/airbnb_data_dictionary.pdf)  

---

## Permasalahan Bisnis
Bangkok merupakan salah satu kota dengan kunjungan wisatawan internasional tertinggi di dunia. Persaingan antar host di platform Airbnb semakin meningkat seiring pertumbuhan jumlah wisatawan. Permasalahan utama yang ingin dijawab melalui analisis ini adalah: faktor apa yang mendorong sebuah listing menjadi lebih populer, mendapatkan lebih banyak pemesanan, serta ulasan positif.  

---

## Metodologi
1. Data Cleaning  
   - Menangani missing values pada variabel ulasan, tanggal, dan nama host  
   - Normalisasi kategorikal pada nama distrik  
   - Deteksi dan evaluasi outlier pada harga, minimum nights, dan jumlah ulasan  

2. Exploratory Data Analysis  
   - Analisis distribusi harga, ketersediaan, tipe kamar, dan lokasi  
   - Segmentasi listing berdasarkan tipe kamar dan distrik  

3. Analisis Statistik  
   - Regresi Poisson untuk menilai pengaruh variabel harga, tipe kamar, ketersediaan, dan minimum nights terhadap jumlah ulasan  
   - Uji Kruskal-Wallis untuk perbedaan ulasan antar distrik dan tipe kamar  
   - Korelasi Spearman untuk mengukur hubungan antara harga, ketersediaan, dan jumlah ulasan  

4. Visualisasi  
   - Visualisasi distribusi dan hubungan variabel menggunakan Python (Matplotlib, Seaborn, Pandas)  
   - Dashboard interaktif dengan Tableau untuk storytelling dan eksplorasi data  

---

## Temuan Utama
- Listing dengan tipe Entire home/apartment cenderung lebih populer dan mendapatkan ulasan lebih banyak dibanding tipe kamar lain.  
- Listing dengan harga kompetitif, khususnya pada kisaran 900–2.500 Baht, memiliki kemungkinan lebih tinggi untuk dipesan.  
- Ketersediaan tinggi sepanjang tahun dan minimum nights yang fleksibel (1–2 malam) berhubungan positif dengan jumlah ulasan.  
- Distrik Khlong Toei, Watthana, Bang Rak, dan Sathorn merupakan area dengan performa listing tertinggi.  

---

## Deliverables
- Notebook Analisis: [airbnb_bangkok_analysis.ipynb](notebooks/airbnb_bangkok_analysis.ipynb)  
- Laporan Presentasi: [presentation-airbnb-listings-bangkok.pdf](reports/presentation-airbnb-listings-bangkok.pdf)  
- Dashboard Tableau: [Link Tableau](https://public.tableau.com/app/profile/liswatun.naimah/viz/LiswatunNaimah-AirbnbBangkok/AirbnbBangkok)  

---

## Rekomendasi
### Untuk Host
- Membuat listing dengan tipe Entire home/apartment untuk menarik lebih banyak peminat.  
- Menetapkan harga kompetitif pada kisaran 900–2.500 Baht, terutama untuk listing baru.  
- Memastikan kalender ketersediaan selalu diperbarui serta menetapkan minimum nights yang fleksibel (1–2 malam).  
- Mengoptimalkan nama listing dengan kata kunci strategis seperti "Near BTS", "Pool", "Central", dan "Wifi" untuk meningkatkan visibilitas pencarian.  

### Untuk Manajemen Airbnb
- Mengoptimalkan algoritma pencarian agar memprioritaskan listing dengan karakteristik yang terbukti populer.  
- Menyediakan rekomendasi otomatis terkait harga dan kata kunci untuk host berdasarkan data distrik.  
- Membuat panduan berbasis data untuk host baru, termasuk strategi penentuan harga dan penulisan deskripsi.  
- Mengembangkan dashboard internal untuk memantau tren pasar dan memberikan wawasan kepada host.  

---

## Kesimpulan
Proyek ini menggambarkan proses analisis data secara menyeluruh, mulai dari pembersihan data, eksplorasi, analisis statistik, hingga visualisasi dan penyusunan strategi bisnis. Hasil analisis ini memberikan gambaran mengenai faktor-faktor utama yang mendorong popularitas listing Airbnb di Bangkok, serta rekomendasi yang dapat diimplementasikan oleh host dan pihak manajemen untuk meningkatkan performa platform.
