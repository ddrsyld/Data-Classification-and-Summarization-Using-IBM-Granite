# Analisis dan Klasifikasi Tingkat Stres Siswa Menggunakan IBM Granite

**Project Overview**

Proyek ini bertujuan untuk menganalisis data publik mengenai stres siswa. Tujuannya adalah untuk memperoleh wawasan yang bernilai mengenai faktor-faktor yang berkontribusi terhadap stres dan mendemonstrasikan bagaimana kecerdasan buatan (AI) dapat digunakan untuk klasifikasi data. Analisis ini menggunakan IBM Granite, sebuah model bahasa besar (LLM), untuk mengklasifikasikan jenis stres berdasarkan indikator yang tersedia dalam data.

**Analis Process**

Proses analisis dilakukan secara sistematis untuk memastikan hasil yang akurat dan relevan.
* Pembersihan Data: Dua dataset CSV dimuat, dan nama kolom pada dataset `Stress_Dataset.csv` dibersihkan untuk mempermudah analisis. Label kategori stres juga disederhanakan.
* Eksplorasi Data (EDA): Analisis statistik dan visualisasi dilakukan untuk memahami distribusi tingkat stres dan faktor-faktor yang berkorelasi dengannya.
* Aplikasi AI: Model IBM Granite diterapkan untuk mengklasifikasikan jenis stres, dengan menggunakan data numerik sebagai fitur masukan.

**Raw Dataset Link**

https://www.kaggle.com/datasets/mdsultanulislamovi/student-stress-monitoring-datasets

**Insight & Findings**

Berdasarkan analisis yang dilakukan, beberapa wawasan penting ditemukan:
* Faktor-Faktor Utama Pemicu Stres: Analisis korelasi menunjukkan bahwa faktor-faktor seperti `anxiety_level`, `depression`, `future_career_concerns`, `peer_pressure`, dan `academic_performance` memiliki korelasi terkuat dengan tingkat stres siswa. Hal ini menunjukkan bahwa intervensi yang menargetkan kesehatan mental dan kekhawatiran akademik memiliki potensi dampak yang paling signifikan.
* Kesenjangan antara Persepsi dan Prediksi AI: Ditemukan bahwa ada kontradiksi antara label stres yang dilaporkan oleh responden (`Eustress` atau stres positif) dan prediksi dari model AI (`Distress` atau stres negatif). Kontradiksi ini bukan merupakan kesalahan model, melainkan sebuah wawasan penting. Model AI mengklasifikasikan stres secara logis berdasarkan indikator objektif seperti `heartbeat_palpitations` dan `anxiety_tension`, sementara label responden mungkin mencerminkan persepsi subyektif mereka terhadap stres sebagai pendorong positif, meskipun indikator fisiknya negatif.

**AI Support Explanation**

AI digunakan secara relevan untuk mendukung analisis proyek ini.
* Pilihan Alat dan Metode: Model IBM Granite dipilih sebagai alat utama karena kemampuannya dalam tugas klasifikasi, yang merupakan salah satu metode yang direkomendasikan dalam panduan proyek.
* Peran AI: Model ini digunakan untuk melakukan klasifikasi jenis stres (Eustress, Distress, atau Tanpa Stres) berdasarkan data numerik yang mewakili kondisi siswa. Hal ini menunjukkan bagaimana LLM dapat digunakan untuk menganalisis data tabular dan membuat kesimpulan yang terstruktur.
