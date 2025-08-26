Sistem Rekomendasi Film menggunakan Neighborhood-Based Collaborative Filtering
Sistem rekomendasi telah menjadi alat penting dalam membantu pengguna menemukan konten yang sesuai dengan preferensi mereka. Namun, dengan banyaknya film yang diproduksi dan beragamnya genre yang tersedia, penonton seringkali kesulitan dalam memilih film yang akan ditonton. Kondisi ini menciptakan kebutuhan akan sistem rekomendasi yang dapat membantu pengguna menemukan film yang relevan.

Tujuan Penelitian
Mengimplementasikan menggunakan model User-Based Collaborative Filtering dalam sistem rekomendasi film.

Mengevaluasi akurasi sistem rekomendasi yang dihasilkan dari model User-Based Collaborative Filtering menggunakan Mean Absolute Error (MAE).

Dataset
Dataset yang digunakan dalam penelitian ini adalah MovieLens 100K, yang tersedia secara publik dari GroupLens Research. Dataset ini sangat ideal untuk penelitian sistem rekomendasi.

Ukuran Dataset: 100.000 rating

Jumlah Pengguna: 943 pengguna unik

Jumlah Film: 1.682 film

Sumber: MovieLens 100K Dataset

Metodologi Penelitian
Penelitian ini menggunakan Neighborhood-Based Collaborative Filtering dengan pendekatan User-Based sebagai metode utama. Detail teknisnya adalah sebagai berikut:

Algoritma: User-Based Collaborative Filtering

Metrik Kemiripan: Cosine Similarity digunakan untuk mengukur seberapa mirip preferensi dua pengguna.

Library: Proyek ini menggunakan scikit-surprise untuk implementasi model.

Optimasi: GridSearchCV digunakan untuk menemukan jumlah tetangga terbaik (K) yang menghasilkan performa optimal.

Evaluasi: Mean Absolute Error (MAE) digunakan untuk mengukur akurasi prediksi model.

Hasil dan Temuan
Setelah serangkaian pengujian, proyek ini menemukan konfigurasi terbaik yang memberikan akurasi tertinggi:

Konfigurasi Terbaik: Skema splitting data 80:20 dengan nilai K = 4.

Akurasi Model: Model mencapai MAE sebesar 0.7236.

Kesimpulan: Nilai MAE yang rendah ini mengindikasikan bahwa sistem rekomendasi yang dikembangkan mampu memprediksi kesalahan kecil dan memberikan rekomendasi yang sangat relevan dengan preferensi pengguna