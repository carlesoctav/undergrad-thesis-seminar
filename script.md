
# awal banget
Selamat pagi Pak Hendri, Bu Nora, Pak Hendri serta teman-teman sekalian. Terima kasih atas kehadirannya di Sidang skripsi saya yang berjudul Aplikasi BERT Pemeringkatan Teks Bahasa Indonesia

Kita masuk pendahuluan

1. Peningkatan jumlah data teks digital membuat manusia kesulitan
dalam memproses informasi secara efektif dan efisien.
1. Tahap pertama dalam memproses informasi dari data teks adalah
melakukan penyimpanan data teks dengan efisien.
1. Diperlukan mekanisme untuk mengembalikan teks yang relevan dari
kumpulan data teks tersebut. Mekanisme pengembalian teks
menjadi semakin penting dengan peningkatan jumlah data teks.

1. Pemeringkatan teks adalah salah satu mekanisme untuk
mengembalikan teks yang relevan.
1. Tujuan dari pemeringkatan teks adalah menghasilkan daftar teks
yang terurut berdasarkan relevansinya terhadap permintaan
pengguna.

Bagan berikut menjelaskan alur pemeringkatan teks, yaitu kumpulan teks akan diberi skor. selanjutnya kumpualan teks tersebut diranking berdasarkan skor yang diperoleh

pada contoh ini, ditunjukkan pemeringkatan teks klasik, dimana fungsi skoring bergantung antara kecocokan antara kata-kata pada kueri dan teks.

Salah satu masalah dari pemeringkatan teks klasik adalah ketika kueri dan teks tidak memiliki kata yang sama. 

1. Kueri apa makanan terenak di Indonesia, dan teks hidangan
terlezat di nusantara adalah rendang tentunya akan
mendapatkan skor yang rendah bila menggunakan fungsi skoring
kecocokan antara kata-kata pada kueri dan teks, karena tidak ada kata yang cocok antara kueri dan teks, meskipun seharusnya teks tersebut relevan dengan kueri.

2. Hal ini diatasi dengan penggunaan fungsi skoring berbasis deep
learning.

diagram alur pemeringkatan yang serupa, namun perbedaan pada fungsi skoring yang digunakan dengan deep learning yang mengatasi masalah vocab mismatch.

Selanjutnya kita masuk ke BERT

Model Bidirectional Encoder Representations from Transformers
(BERT) adalah model pra-latih deep learning yang dikembangkan
oleh Devlin, Chang, Lee, dan Toutanova (2018) untuk permasalahan
bahasa alami. BERT memetakan kata-kata pada kalimat menjadi
representasi vektor yang kontekstual.
2. BERT telah menjadi state-of-the-art untuk berbagai permasalahan
pemrosesan bahasa alami seperti question answering, named entity
recognition, sentiment analysis, dan pemeringkatan teks

Sebagai contoh, dua perusahaan search engine terbesar menggunakan BERT pada mesin pencariaannya.

# pas pemeringkatan teks bahasa inggris

apa yang saya ingin tunjukkan berikut akan menujukkan kontras ketimpangan perkembangan NLP berbahsa Inggris dengan NLP berbahasa Indonesia, khususnya dalam pemeringkatan teks. 

pada gambar ini saya mencari model bert berbahasa inggris untuk "pemeringkatan teks". Terdapat total 339 model dan banyak dari model tersebut terdokumentasi dengan baik performanya.

*next slide*

Bandingkan dengan model-model bert berbahasa Indonesia untuk "pemeringkatan teks". Terdapat 21 model,namun hanya 3 model yang bukan model multibahasa dan tidak ada model yang terdokumentasi dengan baik performanya.

Dari kurangnya model-model BERT berbahasa Indonesia untuk pemeringkatan Teks yang terdokumentasi dengan baik performanya, Skripsi ini dibuat untuk menghasilkan model BERT berbahasa Indonesia yang dapat digunakan untuk pemeringkatan teks dan tentunya ada dokumentasi performa sehingga khalayak umum dapat menggunakan model tersebut dengan percaya diri.


# rumusan masalah dan tujuan
((tujuan kedua dokumentasi))


# Batasan masalah
Sepengetahuan penulis hanya terdapat tiga dataset untuk pemeringkatan teks berbahasa Indonesia.


1. Dataset yang digunakan untuk melatih kembali (fine tuning ) model
BERT adalah dataset mMarco train set bahasa Indonesia
(Bonifacio, Campiotti, de Alencar Lotufo, & Nogueira, 2021).
2. Dataset yang digunakan untuk mengukur performa model adalah
dataset mMarco dev set bahasa Indonesia (Bonifacio et al., 2021)
untuk in-domain test serta MrTyDi dev set bahasa Indonesia
(Zhang, Ma, Shi, & Lin, 2021), dan Miracl dev set bahasa Indonesia
(Zhang et al., 2023) untuk out-of-domain test.
3. Kinerja model diamati dengan metrik recriprocal rank (RR), recall
(R), dan normalized discounted cumulative gain (NDCG).



