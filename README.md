Deskripsi Proyek
Latar Belakang
Project ini bertujuan untuk melakukan segmentasi nasabah berdasarkan data transaksi pada dataset bank_transaction_data. Dengan pendekatan unsupervised learning dan supervised learning, dilakukan proses clustering untuk mengelompokkan data tanpa label, kemudian hasil clustering digunakan sebagai label untuk membangun model klasifikasi.

Alur Proses
1. Clustering Data Transaksi
Tahap awal adalah melakukan clustering pada data transaksi nasabah menggunakan metode unsupervised learning. Proses ini bertujuan untuk mengidentifikasi pola dan mengelompokkan nasabah berdasarkan perilaku transaksi mereka.

2. Analisis Statistik Deskriptif Berdasarkan Cluster
Setelah cluster terbentuk, dilakukan analisis deskriptif untuk memahami karakteristik masing-masing cluster:

Fitur Numerik: Dilakukan analisis statistik deskriptif seperti nilai minimum, maksimum, rata-rata, standar deviasi, dan quartiles menggunakan .describe().

Fitur Kategorikal: Dicari modus (nilai yang paling sering muncul) di setiap fitur kategorikal per cluster.

Visualisasi:

Boxplot: Menampilkan distribusi fitur numerik per cluster.

Countplot: Menampilkan frekuensi fitur kategorikal per cluster.

3. Pemberian Label Berdasarkan Hasil Clustering
Hasil clustering digunakan sebagai label baru pada dataset. Cluster ini menjadi target/label untuk proses supervised learning selanjutnya.

4. Pembangunan Model Klasifikasi
Setelah dataset memiliki label hasil clustering, dilakukan pembangunan model klasifikasi untuk memprediksi cluster berdasarkan data transaksi menggunakan dua algoritma:

K-Nearest Neighbors (KNN)

Random Forest Classifier

Model dilatih menggunakan fitur-fitur transaksi dengan label cluster sebagai target.