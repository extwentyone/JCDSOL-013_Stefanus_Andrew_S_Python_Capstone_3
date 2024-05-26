# JCDSOL-013_Stefanus_Andrew_S_Python_Capstone_3
JCDSOL_CapstoneProject_3_Stefanus_Andrew_Susanto_California Housing Prices 

# California Housing Prices

## Pendahuluan

Selamat datang di California Housing Prices! Proyek ini bertujuan untuk membangun model machine learning yang dapat memprediksi nilai median rumah di California berdasarkan berbagai fitur seperti lokasi, usia rumah, total kamar, total kamar tidur, populasi, rumah tangga, dan pendapatan median. Proyek ini sangat berguna bagi agen real estate, calon pembeli rumah, dan investor yang ingin membuat keputusan yang tepat di pasar perumahan California.

## Masalah Bisnis

Rumah atau properti merupakan kebutuhan utama semua orang. California merupakan salah satu area incaran paling strategis bagi para calon pembeli. Selain untuk kebutuhan utama, rumah juga dapat dijadikan sebuah aset investasi bagi pembeli. Harga pasar pada industri properti (rumah khususnya) di California sangat fluktuatif dan sulit untuk diprediksi. Hal ini menjadi penting untuk para pemangku kepentingan, khususnya agen real estate di California, untuk mengetahui faktor apa saja yang dapat mempengaruhi fluktuasi harga dan bagaimana prediksi terhadap harga rumah yang akan dibeli atau diinvestasikan.

## Tujuan

Tujuan proyek ini ditentukan menggunakan kriteria SMART:

- **Spesifik**: Membangun model machine learning yang dapat memprediksi nilai median rumah di California.
- **Terukur**: Menggunakan metrik Mean Squared Error (MSE) dan R-squared untuk mengukur kinerja model.
- **Dapat Dicapai**: Menggunakan dataset dari sensus California tahun 1990 dan beberapa model machine learning yang telah terbukti efektif dalam prediksi.
- **Relevan**: Memberikan alat prediksi yang berguna bagi pemangku kepentingan dan calon pembeli.
- **Terikat Waktu**: Mencapai model prediksi yang optimal dalam waktu 3 bulan.

## Data

Dataset yang digunakan dalam proyek ini berasal dari sensus California tahun 1990. Dataset ini mencakup informasi tentang berbagai rumah yang ditemukan di distrik California dan beberapa statistik ringkasan. Kolom-kolom dalam dataset adalah sebagai berikut:

- `longitude`: Bujur rumah.
- `latitude`: Lintang rumah.
- `housing_median_age`: Usia median rumah.
- `total_rooms`: Total jumlah kamar di rumah.
- `total_bedrooms`: Total jumlah kamar tidur di rumah.
- `population`: Populasi di blok rumah.
- `households`: Jumlah rumah tangga di blok rumah.
- `median_income`: Pendapatan median rumah tangga di blok rumah.
- `median_house_value`: Nilai median rumah.
- `ocean_proximity`: Kedekatan rumah dengan laut.

## Metodologi

1. **Pemahaman Data**: Memuat dan mengeksplorasi dataset untuk memahami struktur dan isinya.
2. **Pra-pemrosesan Data**: Membersihkan data, menangani nilai yang hilang, dan melakukan rekayasa fitur.
3. **Analisis Data Eksploratif (EDA)**: Menganalisis distribusi data dan korelasi antara fitur-fitur.
4. **Pemodelan**: Membangun dan mengevaluasi beberapa model machine learning (Linear Regression, Decision Tree, Random Forest).
5. **Evaluasi**: Mengevaluasi model menggunakan metrik MSE dan R-squared untuk menentukan model terbaik.
6. **Kesimpulan dan Rekomendasi**: Menarik kesimpulan dari hasil pemodelan dan memberikan rekomendasi untuk perbaikan di masa depan.

## Hasil

- **Linear Regression**: MSE = 4,964,823,650.892547, R-squared = 0.6281319499136326
- **Decision Tree**: MSE = 5,183,186,280.116955, R-squared = 0.6117764676545971
- **Random Forest**: MSE = 2,427,354,086.770494, R-squared = 0.8181898301756912

Model Random Forest memberikan hasil terbaik, menjelaskan sekitar 81.82% variansi dalam nilai median rumah.

## Kesimpulan dan Rekomendasi

Berdasarkan pemodelan yang telah dilakukan, model Random Forest memberikan prediksi yang paling akurat untuk nilai median rumah di California. Fitur `median_income` dan `housing_median_age` adalah faktor yang paling berpengaruh terhadap harga rumah.

### Rekomendasi untuk Pekerjaan Selanjutnya

1. **Mengecek Prediksi dengan Nilai Error Tinggi**: Analisis prediksi dengan error tinggi untuk memahami faktor-faktor yang menyebabkan error dan meningkatkan model.
2. **Penambahan Fitur yang Lebih Korelatif**: Tambahkan fitur seperti luas bangunan, kondisi rumah, dan jarak ke pusat kota untuk meningkatkan akurasi model.
3. **Menggunakan Model yang Lebih Kompleks**: Pertimbangkan penggunaan model yang lebih kompleks seperti Gradient Boosting Machines atau Neural Networks jika ada tambahan data.
4. **Mengembangkan Model Tambahan**: Gunakan model ini untuk mengembangkan model lain seperti memprediksi harga rumah setelah renovasi atau pembangunan baru.

## Struktur Repository

- `Final_California_Housing_Analysis.ipynb`: Notebook Jupyter yang berisi analisis dan proses pemodelan lengkap.
- `README.md`: Pengantar dan dokumentasi proyek.

## Pengakuan

Proyek ini menggunakan data dari sensus California tahun 1990, yang awalnya ditampilkan dalam makalah oleh Pace, R. Kelley, dan Ronald Barry berjudul "Sparse spatial autoregressions" yang diterbitkan di Statistics & Probability Letters 33.3 (1997): 291-297.

