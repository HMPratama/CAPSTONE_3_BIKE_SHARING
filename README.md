# CAPSTONE_3_BIKE_SHARING

*Study case: Bike Sharing*

## **Contents**

1. Business Problem Understanding
2. Data Understanding
3. Data Preprocessing
4. Modeling
5. Conclusion
6. Recommendation

################################################################################################################################################

## **Business Problem Understanding**

### **Introduction**

Perusahaan untuk **bike sharing** seperti perusahaan platform yang telah ada pada kendaraan **Uber** dan **Lyft** merupakan bisnis model yang menyediakan kenyamanan, terjangkau, dan efisien dalam seseorang memilih alat transportasi yang ingin pergi ke tempat yang dituju, tanpa harus memiliki kendaraan. Namun, dengan angka pertumbuhan dari automobiles, sharing kendaraan tidak lagi menjadi efisien terutama pada daerah yang sangat padat dan sibuk di kota besar dan di daerah *Central Business District*. Oleh karena itu, bike sharing merupakan ide yang brilian yang mana menyediakan masyarakat alat transportasi untuk jarak dekat yang mana memudahkan masyarakat untuk sampai tempat tujuan dengan cepat tanpa terjebak kemacetan dan mungkin bisa sambil menikmati pemandangan perkotaan dengan segala keadaan dan aktifitasnya. Kenyataannya, bike sharing merupakan program di USA yang sudah ada 15 tahun sebelum Uber booming.

Bagian yang sangat menarik dari aplikasi dari bike sharing, karakteristik dari data generate denga sistem tersebut membuat mereka tertarik untik melakukan penelitian. tidak seperti pelayanan transportasi lain pada umumnya seperti bus atau subway, yang membutuhkan waktu lebih untuk berpergian kesana kesini dan posisi kedatangan terekam secara eksplisit pada sistem mereka. Fitur pada bike-sharing dilengkapi dengan *virtual sensor network* guna untuk mendeteksi mobilitas dalam kota. Karena itu, hal yang diharapkan bahwa pada keadaan perkotaan dapat mendeteksi dan memonitor data tersebut.

### **Problem Statement**

Salah satu tantangan terbesar yang dihadapi oleh sistem bike-sharing adalah menentukan kondisi seperti apa yang akan menarik banyak calon pengguna untuk menyewa sepedanya. Mengumpulkan data tersebut setiap hari dan mempelajari polanya dapat memberikan manfaat bagi perusahaan dalam memprediksi hari atau musim tertentu dan kondisi apa pun yang menghasilkan calon pengguna dalam jumlah besar.

Terlepas dari segala kemudahan yang diberikan, namun sistem bike sharing masih menghadapi kekurangan pada beberapa aspek yang salah satunya berkaitan dengan kondisi cuaca. Biasanya, cuaca cerah atau berawan akan menarik sebagian besar pengguna untuk menyewa sepeda, sementara kondisi tertentu seperti sedikit kabut dan pemandangan mendung atau mungkin hujan ringan mungkin masih dianggap dapat diterima oleh sebagian pengguna. Namun ketika cuaca ekstrim seperti hujan lebat, badai petir, salju tebal, atau kabut tebal, hampir tidak ada calon pengguna yang mau menyewa sepeda. Faktor lain seperti musim dan perayaan hari libur juga berperan dalam melacak jumlah pengguna yang konsisten setiap hari. Sistem sendiri tidak dapat memprediksi pola pengguna saat ini berdasarkan faktor-faktor yang disebutkan, oleh karena itu sangat penting untuk mempelajari bagaimana faktor-faktor tersebut berkorelasi satu sama lain yang akan menghasilkan banyak calon pengguna dalam menyewa sepedanya.

### **Goals**
Sebagai Data Analyst, Direktur Perusahaan Bike-Sharing selaku pemangku kepentingan diharuskan membangun model Machine Learning yang mampu memprediksi kondisi apa yang paling optimal dalam menarik penyewa dalam jumlah besar berdasarkan faktor-faktor mendasar seperti kondisi cuaca, musim, dan perayaan hari raya. Dengan penggunaan model prediksi yang tepat, dapat membantu perusahaan bike sharing dalam menghasilkan pendapatan dengan mempelajari polanya sekaligus meminimalkan kerugian akibat perawatan sepeda dan potensi risiko akibat insiden vandalisme dan pencurian.

### **Analytic Approach**
Untuk menentukan kondisi seperti apa yang menarik banyak calon pengguna sepeda sewaan, pendekatan yang dilakukan adalah melakukan analisis data untuk menggali dan mengumpulkan pola-pola yang ada dalam data, dilanjutkan dengan menghasilkan model tipe regresi sebagai metode pengujian dalam pengecekan. apakah terdapat korelasi antara berbagai fitur dan jumlah penyewa sepeda dalam bentuk persamaan matematika. Model tipe regresi juga akan digunakan untuk memprediksi kondisi paling optimal dalam menarik penyewa dalam jumlah besar sehingga perusahaan bike sharing dapat memperoleh wawasan tentang berbagai strategi bisnis apa yang dapat diterapkan dalam skenario tersebut yang menguntungkan bagi perusahaan.

### **Metric Evaluation**
Evaluasi metrik yang dipilih untuk model tipe regresi adalah RMSE, MAE, dan MAPE. Root Mean Squared Error (RMSE) adalah akar kuadrat dari mean squared error antara nilai prediksi dan nilai aktual. Mean Absolute Error (MAE) adalah perbedaan absolut rata-rata antara nilai aktual dan nilai prediksi. Mean Absolute Percentage Error (MAPE) adalah rata-rata seluruh persentase kesalahan absolut antara nilai prediksi dan nilai aktual. Semakin kecil nilai RMSE, MAE, dan MAPE maka semakin akurat model dalam melakukan prediksi.



### **Dataset**
Sebelum mengatasi tantangan ini, analisis perlu dilakukan pada kumpulan data. Kumpulan data dapat diakses di sini.

### **Data Understanding**
Dataset terdiri dari sistem bike-sharing mengenai informasi kondisi `Weather`, `Season`, `Holiday`, `Temp`, `Atem`, dan `hr` yang dapat mempengaruhi jumlah penyewa dari tahun 2011 hingga 2012.
