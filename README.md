# Deteksi-Hoaks-Berbahasa-Indonesia

-------------------------------------
Tugas Akhir Sarjana S1 Mahasiswa STMIK LIKMI : Yosef Adrian
---------------------------------------
Dataset yang digunakan berasal dari penelitian sebelumnya yaitu :
Hoax Detection on Indonesian Text using Long Short-Term Memory
- 10.1109/ICOIACT55506.2022.9972086
- https://github.com/zalizaldiy/fake-news-detection
- Rizaldi Yusuf, Suyanto Suyanto
---------------------------------------
Dataset tersebut mengambil sumber dari 3 sumber berita dengan kredibilitas tinggi menurut jurnal tersebut yaitu 
(cnnindonesia, detik.co.id, dan turnbackhoax.id) dengan cara melakukan crawling/scrap data

- Penelitian sebelumnya menggunakan Word2Vec dan LSTM dan proses validasi menggunakan 10-fold-cross-validation score
Didapatkan hasil rata-rata dari keseluruhan sebesar 
- akurasi : 89.42%
- Presisi : 88.76% 
- Recall : 92.53%
- F1-Score : 89.97%
---------------------------------------
Penelitian yang akan saya gunakan dalam deteksi hoaks berbahasa Indonesia kali ini adalah menggunakan :
- Feature Extraction : TFIDF dan n-gram => mengekstrak fitur semantik => telah digunakan pada penelitian-penelitian sebelumnya dalam kasus deteksi hoaks dan mendapatkan akurasi terendah 91% dan tertinggi 98.5%
- Algoritma Klasifikasi : Passive Aggressive Classifier (memiliki performa klasifikasi yang baik dalam kasus deteksi hoaks pada penelitian sebelum-sebelumnya berbahasa Inggris)

Tujuan : 
- Bagaimana performa klasifikasi algoritma passive aggressive classifier dalam melakukan deteksi berita hoaks berbahasa Indonesia?

Penelitian ini akan menggunakan hyperparameter tuning dan k-fold cross-validation :
- Untuk mendapatkan hyperparameter terbaik pada algoritma Passive Aggressive Classifier
- Untuk mengantisipasi overfitting pada model dengan cara melakukan cross validation pada data training (dibagi menjadi data training dan data validation)
- Model yang dihasilkan dari hyperparameter berikut akan diujikan dengan data testing yang tidak disentuh karena khusus untuk proses pengujian

Penelitian ini akan menggunakan evaluasi matrix menggunakan Confusion Matrix :
- Merupakan evaluasi metrik yang umum digunakan
- Deteksi Berita hoaks sering menggunakan evaluasi confusion matrix
- Dapat menghitung akurasi, recall, precision, dan f1-score yang umum ditemui pada jurnal deteksi berita palsu atau berita hoaks
- Tujuan lainnya ialah ingin mengetahui performa seberapa tepat berita hoaks dan tidak hoaks yang terklasifikasi dengan tepat dan tidak tepat

Hasil Akhir (Hipotesis Awal) :
- Penelitian akan menghasilkan hasil performa klasifikasi terbaik menggunakan algoritma PAC
- Algoritma PAC dapat mengalahkan penelitian sebelumnya dengan performa klasifikasi yang lebih baik (Belum Terbukti)
- Menjadi bahan penelitian untuk penelitian berikutnya

Hasil Akhir (Hipotesis Akhir-Pengujian) :
- Nan
