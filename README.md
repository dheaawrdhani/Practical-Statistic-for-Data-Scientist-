# Practical Statistics for Data Scientists

Repository ini berisi reproduksi dan ringkasan **Bab 1 sampai Bab 4** dari buku *Practical Statistics for Data Scientists* (Bruce, Bruce & Gedeck, O'Reilly). Setiap bab dibuat dalam satu notebook Jupyter/Colab yang berisi:

1. **Kode** dari buku yang dijalankan ulang dengan Python.
2. **Penjelasan teori** dalam bahasa Indonesia di hampir setiap sel kode (apa yang dilakukan kode, cara membaca hasilnya, dan kesimpulannya).
3. **Ringkasan bab** pada bagian awal atau di sela-sela notebook.

## Ringkasan Tiap Bab

### Bab 1: Exploratory Data Analysis (EDA)

EDA adalah langkah pertama di setiap proyek data science: melihat dan meringkas data sebelum membuat model. Bab ini mengajarkan cara meringkas data dengan angka dan grafik.

- **Ukuran pemusatan (location):** mean, trimmed mean, weighted mean, median, dan weighted median. Median dan trimmed mean lebih tahan terhadap nilai ekstrem (outlier) daripada mean.
- **Ukuran penyebaran (variability):** standar deviasi, IQR (rentang antar-kuartil), dan MAD (median absolute deviation).
- **Bentuk distribusi:** persentil, boxplot, tabel frekuensi, histogram, dan density plot.
- **Data biner dan kategori:** proporsi dan diagram batang, dengan contoh penyebab keterlambatan penerbangan di bandara DFW.
- **Korelasi:** koefisien korelasi, matriks korelasi, heatmap, dan ellipse plot pada harga saham dan ETF.
- **Dua variabel atau lebih:** scatter plot, hexagonal binning, contour plot, tabel kontingensi (grade vs status pinjaman), boxplot per kategori, violin plot, dan faceting.

**Dataset:** data penduduk dan murder rate negara bagian AS, keterlambatan bandara DFW, harga saham S&P 500, pajak properti King County, pinjaman Lending Club, dan statistik maskapai.

### Bab 2: Data and Sampling Distributions

Bab ini menjelaskan hubungan antara **sampel** dan **populasi**, serta mengapa hasil dari sampel selalu mengandung ketidakpastian.

- **Sampling dan bias:** sampel yang bagus harus acak, cukup besar, dan bebas bias. Kualitas sampel lebih penting daripada sekadar banyaknya data.
- **Distribusi sampling:** distribusi suatu statistik (misalnya rata-rata) dari banyak sampel. Rata-rata dari sampel berukuran 20 lebih sempit dan lebih berbentuk lonceng daripada rata-rata sampel berukuran 5, dan lebih sempit daripada data individu.
- **Bootstrap:** resampling dengan pengembalian untuk memperkirakan bias dan standard error suatu statistik (contoh: median pendapatan peminjam dengan standard error sekitar 229).
- **Selang kepercayaan (confidence interval):** dibuat dengan bootstrap pada tingkat 90% dan 95%.
- **Distribusi normal dan QQ plot:** cara mengecek apakah data normal. Return saham NFLX ternyata punya ekor yang lebih berat daripada normal.
- **Distribusi lain:** binomial, Poisson, eksponensial, dan Weibull, beserta kapan masing-masing dipakai.

### Bab 3: Statistical Experiments and Significance Testing

Bab ini membahas cara menguji apakah perbedaan yang terlihat di data benar-benar nyata atau hanya kebetulan.

- **A/B test:** membandingkan dua perlakuan, misalnya dua halaman web atau dua harga.
- **Permutation test:** mengacak label kelompok ribuan kali untuk melihat seberapa sering selisih sebesar yang teramati muncul karena kebetulan.
- **p-value dan signifikansi:** perbedaan lama kunjungan Page A dan B (p sekitar 0,12) serta conversion rate dua harga (p sekitar 0,33) tidak signifikan.
- **t-test:** uji beda dua rata-rata dengan rumus, hasilnya mirip dengan permutation test.
- **ANOVA:** uji beda rata-rata untuk lebih dari dua kelompok (empat halaman web).
- **Chi-square:** menguji apakah klik tiga judul berita berbeda, dengan resampling maupun rumus.
- **Power dan ukuran sampel:** untuk mendeteksi selisih kecil dibutuhkan sampel sangat besar (sekitar 116.600 per kelompok untuk kenaikan 10%), sedangkan selisih besar butuh jauh lebih sedikit (sekitar 5.500).

**Dataset:** waktu kunjungan halaman web, empat sesi halaman, klik judul berita, dan data Imanishi.

### Bab 4: Regression and Prediction

Bab ini membahas regresi untuk memprediksi nilai numerik dan memahami hubungan antar variabel.

- **Regresi linear sederhana dan berganda:** koefisien, intercept, nilai prediksi, dan residual.
- **Menilai model:** RMSE, R², p-value, dan interval kepercayaan koefisien.
- **Seleksi variabel:** stepwise berdasarkan AIC, untuk memilih variabel yang benar-benar berguna.
- **Regresi berbobot:** memberi bobot lebih pada data yang lebih baru.
- **Variabel kategori:** one-hot encoding dengan kategori pembanding, serta cara mengelompokkan variabel dengan banyak nilai seperti kode pos.
- **Menafsirkan regresi:** prediktor yang saling berkorelasi (multikolinearitas), confounding, dan interaksi antar variabel.
- **Diagnostik regresi:** outlier, residual terbakukan, data berpengaruh (hat value dan Cook's distance), heteroskedastisitas, dan partial residual plot.
- **Hubungan non-linear:** regresi polinomial, spline, dan GAM (Generalized Additive Model).
- **Regularisasi:** Lasso yang mengecilkan koefisien dan membuang variabel yang kurang berguna.

---

## Sumber

Kode dan dataset berasal dari repository resmi buku:
[gedeck/practical-statistics-for-data-scientists](https://github.com/gedeck/practical-statistics-for-data-scientists)

> Bruce, P., Bruce, A., & Gedeck, P. *Practical Statistics for Data Scientists*. O'Reilly Media.

Repository ini dibuat untuk tugas dan catatan belajar. Hak cipta buku dan kode aslinya tetap milik penulisnya. Penjelasan teori dalam bahasa Indonesia dibuat dengan bantuan LLM dan sebaiknya diperiksa kembali dengan buku.

## Author
Dhea Kusuma Wardhani
