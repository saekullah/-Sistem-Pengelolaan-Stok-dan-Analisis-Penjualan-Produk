# 01. Pengenalan Proyek

## 1.1 Latar belakang

Pengelolaan stok merupakan salah satu kegiatan penting dalam bisnis ritel. Pemilik toko perlu mengetahui produk yang banyak diminati, produk yang jarang terjual, dan pendapatan yang dihasilkan setiap produk. Jika keputusan hanya mengandalkan perkiraan, toko dapat mengalami kelebihan stok atau kehabisan barang.

Data transaksi yang dikumpulkan secara rutin dapat diolah untuk menemukan pola penjualan. Data Mining membantu mengubah data tersebut menjadi informasi yang mendukung keputusan.

## 1.2 Identifikasi masalah

1. Sulit mengetahui performa setiap produk jika transaksi sudah banyak.
2. Produk yang sering terjual dan produk yang kurang diminati belum tentu mudah dikenali tanpa ringkasan data.
3. Keputusan promosi dan pengelolaan stok dapat kurang tepat jika tidak didukung analisis.
4. Data transaksi perlu dibersihkan dan diolah sebelum digunakan untuk analisis.

## 1.3 Rumusan masalah

- Bagaimana menyiapkan data penjualan agar layak dianalisis?
- Produk apa yang memiliki jumlah penjualan dan pendapatan relatif tinggi atau rendah?
- Bagaimana K-Means dapat digunakan untuk mengelompokkan produk berdasarkan performa penjualan?
- Bagaimana hasil analisis dapat diterjemahkan menjadi rekomendasi pengelolaan stok?

## 1.4 Tujuan

- Melakukan preprocessing terhadap dataset penjualan.
- Menganalisis jumlah penjualan dan pendapatan per produk.
- Mengimplementasikan clustering K-Means.
- Mengevaluasi dan menginterpretasikan hasil clustering.
- Menyusun rekomendasi awal untuk membantu pengelolaan stok.

## 1.5 Ruang lingkup

Proyek ini menggunakan dataset CSV contoh yang berisi transaksi penjualan produk. Fokus utama adalah analisis penjualan dan pengelompokan produk, bukan aplikasi kasir lengkap. Data stok, pemasok, biaya operasional, dan masa kedaluwarsa belum menjadi bagian dari dataset utama.

## 1.6 Manfaat

- **Pembelajaran:** memahami alur proyek Data Mining dari awal sampai akhir.
- **Operasional:** memberi gambaran performa penjualan produk.
- **Pengembangan:** menjadi dasar pembuatan dashboard atau sistem stok yang lebih lengkap.

## 1.7 Indikator keberhasilan

1. Dataset dapat dibaca dan diperiksa dengan benar.
2. Statistik penjualan per produk berhasil dihitung.
3. Model K-Means menghasilkan label cluster.
4. Hasil cluster dapat dijelaskan menggunakan nilai rata-rata fitur.
5. Grafik dan file hasil analisis berhasil dibuat.
