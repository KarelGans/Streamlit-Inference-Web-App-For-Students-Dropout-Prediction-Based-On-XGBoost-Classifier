# Proyek Akhir: Menyelesaikan Permasalahan Perusahaan Edutech - Deteksi Dini Siswa Dropout di Jaya Jaya Institut

## Business Understanding
Jaya Jaya Institut, berdiri sejak tahun 2000, merupakan institusi pendidikan tinggi yang telah menghasilkan banyak lulusan dengan reputasi sangat baik. Meskipun demikian, institusi ini menghadapi tantangan signifikan terkait tingginya angka siswa yang tidak menyelesaikan pendidikannya (dropout). Jumlah dropout yang tinggi menjadi masalah besar karena dapat mempengaruhi reputasi institusi, efisiensi operasional, serta potensi pendapatan di masa depan. Oleh karena itu, Jaya Jaya Institut berkeinginan untuk dapat mendeteksi sedini mungkin siswa-siswa yang berpotensi melakukan dropout agar dapat diberikan perhatian dan bimbingan khusus, sehingga angka dropout dapat ditekan.

### Permasalahan Bisnis

Permasalahan utama yang dihadapi oleh Jaya Jaya Institut adalah:
1.  **Tingginya angka dropout siswa:** Banyak siswa yang tidak berhasil menyelesaikan pendidikannya, yang berdampak negatif pada berbagai aspek institusi.
2.  **Kurangnya sistem deteksi dini:** Belum ada mekanisme yang efektif untuk mengidentifikasi siswa yang berpotensi dropout secara proaktif.
3.  **Kebutuhan intervensi yang tepat sasaran:** Tanpa deteksi dini, sulit untuk memberikan bimbingan atau intervensi yang tepat waktu dan tepat sasaran kepada siswa yang membutuhkan.

### Cakupan Proyek
Proyek ini bertujuan untuk membantu Jaya Jaya Institut dalam mengatasi permasalahan dropout siswa dengan cakupan sebagai berikut:
1.  **Analisis Data Eksploratif (EDA):** Memahami karakteristik siswa dan faktor-faktor yang berkorelasi dengan status kelulusan atau dropout dari dataset yang disediakan.
2.  **Pengembangan Model Machine Learning:** Membangun model klasifikasi untuk memprediksi kemungkinan seorang siswa akan dropout berdasarkan data historis dan atribut siswa.
3.  **Pembuatan Business Dashboard:** Merancang dan mengembangkan dashboard interaktif untuk memvisualisasikan data performa siswa, tren dropout, dan hasil prediksi model. Dashboard ini akan membantu pihak manajemen dalam memantau kondisi siswa dan mengambil keputusan berbasis data.
4.  **Penyusunan Rekomendasi(action items):** Memberikan rekomendasi tindakan yang dapat diambil oleh institusi berdasarkan temuan dari analisis data dan performa model.

### Persiapan

Dataset student Jaya Jaya Institut dapat diakses melalui tautan berikut: [Dataset Mahasiswa Jaya Jaya Institut](*https://github.com/dicodingacademy/dicoding_dataset/blob/main/students_performance/README.md*) 
Setup environment untuk menjalankan jupyter notebook atau model:

```python
# requirements-ipynb.txt
Download lib diatas dengan pip install -r requirements-ipynb.txt
```

## Business Dashboard
Buisness dashboard dibuka melalui tautan : [Dashboard](*https://public.tableau.com/app/profile/carolus.christadi/viz/student_dashboard_tableau/Dashboard1?publish=yes*)

## Menjalankan Sistem Machine Learning
Sistem inference machine learning dibuat di [Streamlit Cloud app](*https://dropout-prediction-based-on-xgboost-classifier.streamlit.app*)
Untuk melakukan running di environment lokal, dapat menjalankan setup environment:

```python
# requirements.txt
Download lib diatas dengan pip install -r requirements.txt
```
Ketika sudah melakukan running app.py, kita perlu melakukan 

```python
streamlit run app.py
```

## Conclusion
Project ini bertujuan untuk uk mengatasi masalah tingginya angka dropout di Jaya Jaya Institut dengan mengembangkan solusi berbasis data. Melalui analisis data yang mendalam, berhasil diidentifikasi faktor-faktor kunci yang berkontribusi terhadap kecenderungan siswa untuk dropout. Selanjutnya, model machine learning telah dikembangkan untuk memprediksi siswa yang berisiko dropout dengan akurasi 92% tanpa adanya indikasi overfitting.

### Rekomendasi Action Items
Berikut merupakan action items dari hasil analisa yang dibuat.

- Melakukan pengecekan terlebih pada siswa-siswi yang memiliki nilai rendah di curriculum karena perbedaan yang terlhat pada dashboard menunjukan nilai rendah cenderung untuk dropout. Oleh karena itu, perlu diperhatikan oleh dosen-dosen agar dapat mengangkat nilai dengan memberikan extra lessons.

- Perlu diperhatikan untuk siswa-siswi yang memiliki tuition fee menunggak.

- Pada data dapat dilihat usia yang lebih tua cenderung untuk dropout sehingga dapat membatasi dengan minimal umur atau memberikan beasiswa kepada yang memiliki umur wajar agar lebih banyak siswa-siswi bekemampuan dan umur yang optimal.

