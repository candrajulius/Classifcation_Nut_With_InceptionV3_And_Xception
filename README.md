# Classifcation Beans With Inception and Xception Architectures(Mengklasifikasi Kacangn Dengan Arsitektur Inception dan Xception)
Membuat sebuah klasifikasi kacangn dengan CNN menggunakan arsitektur InceptionV3 dan Xception

# Business Understanding
***
### Problem Statement
----
### Goals
***
Tujuan dibuatnya proyek ini adalah sebagai berikut:
* Mengahasilkan sebuah klasifikasi kacang dengan berdasarkan akurasi yang tinggi dari dataset yang digunakan
### Solution Approach
***
Solusi yang dapat dilakukan untuk memenuhi tujuan dari proyek ini diantaranya:

__Klasifikasi Berdasarkan Gambar Dengan CNN__
Adalah sebuah proses pengelompokkan data ke dalam beberapa kategori agar lebih mudah untuk diolah dan dianalisis
Konsep dari Classification ini adalah mempelajari gambar dengan memberikan label pada gambar tersebut dan mengelompokkan gambar tersebut berdasarkan label yang telah diberikan

### Arsitektur CNN Yang Digunakan
Berikut adalah arsitektur yang digunakan dalam CNN: 
__InceptionV3__ adalah Arsitektur CNN merupakan gabungan seluruh perbaikan dari InceptionV2
__Xception__ adalah arsitektur jaringan saraf konvolusional mendalam yang melibatkan Konvolusional mendalam yang melibatkan konvolusi Depthwise Separable;

### Data Undestanding
Dataset ini dapat diakses menggunakan [Kaggle 11 Peanut](https://www.kaggle.com/datasets/ruopengan/11-common-nut-types-for-image-classification)
informasi dari dataset dapat dirangkum sebagai berikut
tabel 1: Ringkasan informasi dataset
|   Jenis   |         Ketergangan                                                                                                                   |
|-----------|---------------------------------------------------------------------------------------------------------------------------------------|
|   Sumber  | [11-common-nut-types-for-image-classification](https://www.kaggle.com/datasets/ruopengan/11-common-nut-types-for-image-classification)|
| Lisensi   | CC0: Public Domain |
| Kategori  | Nuts |
| Jenis & Ukuran| Image/File |

Pada berkas yang diunduh terdapat beberapa folder yang berisikan gambar, Untuk penjelasannya dapat dilihat di keterangan di bawah ini;

Pada berkas 11-common-nut-types-for-image-classification terdapat 1320 dataset yang berisikan gambar. Di dalam berkas tersebut ada beberapa folder yang terdiri dari 3 folder
folder val, folder train. folder test, Disini penulis hanya menggunakan folder train. Dimana folder train tersebut memiliki 1320 dataset.

### **Pra-pemrosesan Data**
Pada pra-pemrosesan data dapat dilakukan beberapa tahap, antara lain:
* Memasukkan dataset kedalam direktori collab dengan menggunakan API kaggle
* Setelah itu mengekstrak zip file yang telah masuk kedirectori collab
* Setelah mengekstrak lalu menghitung jumlah dataset pada folder train
* Memvisualisasikan data gambar dan label pada dataset

### **Data Prepation (Menyiapkan Data)**
Pada memvisualisasi data dapat dilakukan beberapa tahap, antara lain:
* Memmbuat direktori train dan val setelah itu menggabungkan setiap sub direktori kedalam train dan val
* Melihat jumlah data gambar pada setiap subdirektori
* Membuat direktori train dan validation dir
* Setelah itu menyambungkan direktori train dan validation dir dengan subdirektori yang telah didefinisikan
* Memvalidasi setiap direktori menjadi data train dan data validasi dengan validation 40% dataset

### **Image Processing**
Pada image processing data dapat dilakukan beberapa tahap, antara lain:
* Melakukan augmentasi pada gambar data train dan data validasi
* Memuat data latih dalam bentuk batch dan melakukan augmentasi gambar secara real-time menggunakan objek yang telah didefinisikan

### **Model Development**
Pada model development dengan arsitektur Xception dan InceptionV3 dapat dilakukan beberapa tahapan, antara lain:
* Membuat model dengan arsitektur InceptionV3 dan Xception
* Melihat arsitektur CNN dengan arsitekur yang digunakan
* Melakukan pelatihan terhadap model
