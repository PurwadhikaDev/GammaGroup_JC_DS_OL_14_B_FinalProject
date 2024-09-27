# CHURN PREDICTION IN TELECOM SECTOR
## Gamma Team
1. Muhammad Raihan
2. Rahmah Anggita Fitri
3. Sandra Helenna Mulyadi

# Business Understanding
Dataset ini berisi informasi mengenai pelanggan yang dapat digunakan untuk memprediksi perilaku mereka dalam rangka meningkatkan tingkat retensi. Meningkatkan retensi berarti menerapkan strategi dan tindakan yang dilakukan oleh perusahaan untuk memastikan pelanggan tetap menggunakan produk atau layanan mereka dalam jangka panjang.
Tujuan dari inisiatif ini adalah untuk mengurangi tingkat churn (penghentian langganan) dan mempertahankan pelanggan yang ada, karena menurut Tjiptono (2009) menjaga pelanggan setia sering kali lebih efektif dan hemat biaya dibandingkan menarik pelanggan baru.
Dalam konteks bisnis, strategi retensi dapat meliputi peningkatan layanan, personalisasi pengalaman pelanggan, program loyalitas, komunikasi yang lebih efektif, serta analisis perilaku pelanggan untuk memahami kebutuhan mereka dengan lebih mendalam.
(source: https://bbs.binus.ac.id/gbm/2019/02/26/customer-retention-2/)

Setiap baris dalam dataset merepresentasikan seorang pelanggan, dengan kolom yang berisi atribut terkait. Data ini mencakup informasi tentang pelanggan yang berhenti berlangganan dalam satu bulan terakhir (kolom "Churn"), serta rincian layanan yang digunakan, seperti layanan telepon, internet, dan streaming. Informasi akun meliputi durasi berlangganan, jenis kontrak, metode pembayaran, penggunaan penagihan tanpa kertas, jumlah tagihan bulanan, dan total tagihan. Data demografis juga tersedia, termasuk jenis kelamin, rentang usia, serta status pernikahan dan tanggungan pelanggan. Informasi ini dapat menganalisis faktor-faktor yang mempengaruhi pelanggan untuk berhenti atau melanjutkan layanan, membantu perusahaan merancang program retensi yang lebih efektif.

# Problem Statement
- Bagaimana profil demografis customer yang paling umum berpotensi untuk churn?
- Bagaimana hubungan tingkat churn customer dengan variabel lain?
- Bagaimana hubungan antar variabel?
- Bagaimana perusahaan bisa memprediksi pelanggan baru yang berpotensi untuk churn dengan model machine learning?

# Objectives
- Memahami profil customer terkait tingkat churn.
- Merancang strategi retensi pelanggan yang lebih efektif dan tepat sasaran, seperti penawaran khusus, peningkatan layanan, atau personalisasi pengalaman, untuk mengurangi tingkat churn.
- Mengembangkan model prediksi yang akurat untuk mengidentifikasi pelanggan yang berisiko melakukan churn, berdasarkan data demografis, layanan yang digunakan, dan perilaku berlangganan.
- Meningkatkan profitability perusahaan dengan reduksi cost dengan mencegah terjadinya loss oleh pelanggan diprediksi yang berpotensi churn.

# Evaluation Metrics
Metric terbaik untuk mempertahankan pelanggan dengan tujuan meminimalkan churn akan bergantung pada prioritas bisnis: apakah fokus pada mendeteksi sebanyak mungkin pelanggan yang mungkin churn atau mengoptimalkan penggunaan sumber daya untuk mencegah churn. Maka Metrics yang kami gunakan adalah : 

**Recall (Sensitivity / True Positive Rate)**
Definisi: Persentase pelanggan yang benar-benar churn dan berhasil diprediksi churn oleh model dengan meminimalkan FN.
Alasan: Jika tujuan utama adalah meminimalkan churn, fokus utamanya adalah memastikan bahwa sebanyak mungkin pelanggan yang benar-benar akan churn dapat teridentifikasi oleh model. Dengan recall yang tinggi, perusahaan dapat menangkap pelanggan yang berisiko tinggi churn dan memberikan perhatian atau insentif agar mereka tidak pergi.


# Exploratory Data Analysis
Berikut feature dari dataset yang kami miliki :

![image](https://github.com/user-attachments/assets/2638aec5-4020-46b8-9b86-87c83ae1cbe3)

Dari dataset tersebut, kami melakukan data cleaning sebelum melakukan data analysis dan modelling. Berikut tahapan cleaning yang kami lakukan :
1. Missing values
2. Outliers
3. Data formatting
4. Data duplicates

# Data Analysis
Dalam tahapan ini, kami melakukan beberapa analisis terhadap dataset. Diantaranya adalah :
1. Data distribution
2. Churn distribution
3. Demographic distribution (Gender dan Seniior Citizen)
4. Hubungan tingkat churn terhadap feature pada dataset
5. Bivariate analysis pada `MonthlyCharges` x `TotalCharges` dan `TotalCharges` x `Contract`
6. Korelasi variabel kategorik terhadap churn
7. Korelasi variabel numerik terhadap churn

# Tableau Dashboard
Hasil dari Data Analysis, kami tuangkan ke dalam Dashboard yang dapat memberikan informasi secara menyeluruh terhadap dataset. Sehingga pembaca bisa lebih mudah memahami dataset. Berikut dashboard yang kami buat 
![image](https://github.com/user-attachments/assets/e045cbc1-d3af-4bd4-ad78-78d22588aa5d)

# Feature Engineering
Hasil dari korelasi antar variabel terhadap churn, kami memutuskan untuk melakukan drop terhadap 3 variabel yaitu `CustomerID`, `gender`, `PhoneService`.
Selain itu, kami juga melakukan pengujian terhadap imbalance dataset yang hasilnya bahwa dataset ini adalah **imbalance** dengan nilai :
- Nilai Churn 0 = 73.42%
- Nilai Churn 1 = 26.58%

# Modelling
Pada tahapan ini, kami menguji beberapa model untuk mendapatkan nilai metrics yang paling baik. Kami juga membuat model panalized dan oversampling karena dataset imbalance.
Setelah itu, kami melakukan hyperparameter tunning pada model terbaik yang hasilnya adalah :

- Model : Logistic Regression
- Oversampling : BorderlineSMOTE
- Parameter C : 2
- Parameter Penalty : l1
- Parameter Solver : saga
- Parameter Class Weight = balanced

Model tersebut menghasilkan **recall sebesar 83.96%**


# Let me know if you need any further adjustments!
**Member:**
1. Muhammad Raihan (muhammadraihan4@gmail.com)
2. Rahmah Anggita Fitri (rahmahanggita@gmail.com)
3. Sandra Helenna Mulyadi (sandrahln43@gmail.com)


# Thank You! 
