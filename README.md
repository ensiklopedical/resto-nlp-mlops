# Submission 1: Sentiment Analysis: Restaurant Review
Nama:

Username dicoding: faisal_ag_037

| | Deskripsi |
| ----------- | ----------- |
| Dataset | [❤️ vs 😡: Sentiment Analysis 📝](https://www.kaggle.com/datasets/mohidabdulrehman/vs-sentiment-analysis) |
| Masalah | masalah utama yang diangkat adalah review dari pengunjung restoran. Review ini berisi opini dan pengalaman pengunjung mengenai berbagai aspek layanan restoran, seperti kualitas makanan, pelayanan, suasana, harga, dan kebersihan. Mengingat review ini sering kali memengaruhi reputasi restoran dan keputusan pelanggan potensial, memahami sentimen yang terkandung di dalamnya menjadi sangat penting. Melalui analisis ini, kami bertujuan untuk mengidentifikasi pola sentimen positif atau negatif dalam ulasan tersebut, yang nantinya dapat digunakan oleh manajemen restoran untuk meningkatkan kualitas layanan dan kepuasan pelanggan. |
| Solusi machine learning | Solusi machine learning yang diterapkan adalah membuat model klasifikasi menggunakan Neural Network (NN) dalam sebuah pipeline. Pipeline memproses data lalu digunakan sebagai input untuk model NN yang terdiri dari beberapa lapisan untuk menangkap dan menganalisis pola sentimen. Model ini dilatih untuk memprediksi apakah review memiliki sentimen positif atau negatif, membantu restoran memahami umpan balik pelanggan secara lebih efektif.|
| Metode pengolahan | 
Metode pengolahan data dalam proyek ini mengikuti urutan langkah yang terstruktur. Pertama, Data Ingestion dilakukan menggunakan ExampleGen untuk mengimpor data. Selanjutnya, Data Validation mencakup StatisticGen untuk menghasilkan statistik data, SchemaGen untuk menentukan skema, dan ExampleValidator untuk memverifikasi integritas data. Kemudian, Data Preprocessing dilakukan dengan Transform untuk menyiapkan data sebelum pelatihan model. Dalam tahap Model Development, Trainer digunakan untuk melatih model dengan data yang telah diproses. Setelah itu, Analysis and Validating the Model dilakukan menggunakan Resolver untuk menangani masalah dan Evaluator untuk menilai kinerja model. Terakhir, model yang telah divalidasi dapat dideploy menggunakan Pusher. |
| Arsitektur model | Arsitektur model yang digunakan dalam proyek ini adalah Neural Network (NN) dengan beberapa lapisan utama. Model dimulai dengan Input Layer yang menerima data teks yang telah diproses. Kemudian, terdapat Embedding Layer yang mengubah teks menjadi representasi vektor berdimensi tetap untuk menangkap makna semantik dari kata-kata. Selanjutnya, Global Average Pooling Layer digunakan untuk mereduksi dimensi data dengan mengambil rata-rata dari embedding, yang membantu menyatukan informasi penting dari teks. Setelah itu, terdapat beberapa Dense Layers dengan aktivasi ReLU yang berfungsi untuk mempelajari pola-pola kompleks dalam data. Terakhir, model memiliki Output Layer dengan aktivasi sigmoid untuk menghasilkan output berupa probabilitas dari dua kelas, yaitu sentimen positif atau negatif. Arsitektur ini dirancang untuk menangkap informasi penting dari teks dan memprediksi sentimen dengan akurat |
| Metrik evaluasi | Untuk mengevaluasi performa model, digunakan metrik binary accuracy dan validation binary accuracy. Binary accuracy mengukur seberapa akurat model dalam memprediksi label sentimen yang benar pada data pelatihan, sementara validation binary accuracy mengukur keakuratan model pada data validasi, membantu memastikan bahwa model dapat menggeneralisasi dengan baik pada data yang belum pernah dilihat. Kedua metrik ini memberikan gambaran yang jelas tentang kemampuan model dalam mengklasifikasikan sentimen secara efektif. |
| Performa model | Performa model menunjukkan hasil yang cukup baik, dengan binary accuracy mencapai 94% pada data pelatihan, yang menunjukkan tingkat akurasi tinggi dalam memprediksi sentimen yang benar. Namun, validation binary accuracy adalah 75%, yang mengindikasikan bahwa meskipun model bekerja sangat baik pada data pelatihan, ada penurunan akurasi saat diterapkan pada data validasi. Hal ini dapat menunjukkan adanya perbedaan antara data pelatihan dan validasi, atau potensi masalah overfitting yang perlu ditangani untuk meningkatkan kemampuan model dalam generalisasi. |
