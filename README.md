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

# Tableau Dashboard
![image](https://github.com/user-attachments/assets/e045cbc1-d3af-4bd4-ad78-78d22588aa5d)

Dashboard diatas berisikan informasi dari dataset yang kami miliki. Dapat dilihat bahwa
