# Sistem Pengelolaan Stok dan Analisis Penjualan Produk

**Proyek pembelajaran Data Mining — studi kasus minimarket fiktif Mriki Mart**

Repository ini mendokumentasikan proses pembelajaran Data Mining dari tahap memahami masalah, menyiapkan dataset, membersihkan data, melakukan analisis eksploratif, menerapkan algoritma K-Means, mengevaluasi model, hingga menyusun rekomendasi pengelolaan stok.

> **Catatan:** Dataset di repository ini adalah data contoh sintetis untuk pembelajaran, bukan data transaksi toko sungguhan.

## Tujuan proyek

1. Memahami pola penjualan produk berdasarkan data transaksi.
2. Mengetahui produk dengan penjualan dan pendapatan relatif tinggi atau rendah.
3. Mengelompokkan produk menggunakan algoritma K-Means.
4. Menggunakan hasil analisis sebagai salah satu bahan pertimbangan pengelolaan stok.
5. Mempelajari alur kerja proyek Data Mining secara terstruktur.

## Teknologi

- Python
- Pandas dan NumPy
- Matplotlib
- Scikit-learn
- CSV sebagai format dataset

## Struktur repository

```text
sistem-pengelolaan-stok-analisis-penjualan/
├── README.md
├── requirements.txt
├── data/
│   └── penjualan_produk.csv
├── docs/
│   ├── 01-pengenalan-proyek.md
│   ├── 02-dasar-data-mining.md
│   ├── 03-metodologi-crisp-dm.md
│   ├── 04-pemahaman-data.md
│   ├── 05-pengumpulan-data.md
│   ├── 06-data-preprocessing.md
│   ├── 07-analisis-eksploratif.md
│   ├── 08-feature-engineering.md
│   ├── 09-algoritma-k-means.md
│   ├── 10-evaluasi-model.md
│   ├── 11-interpretasi-hasil.md
│   ├── 12-rekomendasi-stok.md
│   ├── 13-kesimpulan-dan-pengembangan.md
│   └── 14-publikasi-github.md
├── src/
│   └── analisis_penjualan.py
└── outputs/
    └── README.md
```

## Cara menjalankan

### 1. Siapkan Python

Gunakan Python 3.10 atau lebih baru. Disarankan membuat virtual environment.

```bash
python -m venv .venv
```

Aktifkan environment:

- Windows: `.venv\Scripts\activate`
- macOS/Linux: `source .venv/bin/activate`

### 2. Instal library

```bash
pip install -r requirements.txt
```

### 3. Jalankan analisis

Dari direktori utama repository:

```bash
python src/analisis_penjualan.py
```

Program akan membaca `data/penjualan_produk.csv`, menampilkan ringkasan analisis, dan menyimpan hasil CSV serta grafik ke folder `outputs/`.

## Alur analisis

1. Membaca data transaksi.
2. Memeriksa tipe data, nilai kosong, dan duplikasi.
3. Menghitung jumlah terjual dan pendapatan per produk.
4. Membuat fitur numerik dan melakukan standardisasi.
5. Menjalankan K-Means untuk membentuk tiga kelompok.
6. Menghitung Silhouette Score jika kondisi data memungkinkan.
7. Menyimpan hasil pengelompokan dan grafik.

## Penting saat membaca hasil

Label cluster `0`, `1`, dan `2` yang dihasilkan algoritma **bukan** urutan kualitas. Nama seperti “penjualan tinggi”, “menengah”, dan “rendah” harus ditentukan setelah membandingkan rata-rata penjualan atau pendapatan tiap cluster.

K-Means menemukan kemiripan berdasarkan fitur yang digunakan. Hasilnya bukan ramalan penjualan dan tidak otomatis menentukan jumlah stok ideal. Keputusan stok juga perlu mempertimbangkan stok saat ini, waktu tunggu pemasok, masa kedaluwarsa, pola musiman, dan batas minimum stok.

## Materi pembelajaran

Baca dokumen pada folder [`docs/`](docs/) secara berurutan dari 01 sampai 14.

## Pengembangan berikutnya

- Menambahkan tabel stok saat ini dan data barang masuk.
- Membangun dashboard menggunakan Streamlit.
- Membuat peramalan permintaan dengan data historis yang cukup.
- Menambahkan pengujian model dan validasi dengan data periode berbeda.
- Menghubungkan aplikasi dengan database MySQL.

## Penulis

Nama: *Isi nama kamu*  
Program Studi: Informatika  
Topik: Data Mining dan analisis penjualan produk
