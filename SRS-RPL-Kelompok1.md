<html>
<body><div align="center"><h1>Software Requirement Specification</h1></div>
<p align="center"><b>Version 1.0 </b><br>
<p align="center">23 Maret 2018<br><br>
<p align="center">
<img src="http://i67.tinypic.com/mwba89.png"/>
</p>

<br><p align="center"><b> APLIKASI SISTEM PENYEWAAN KENDARAAN BESERTA RUTE PERJALANAN (ALIKHA EXPRESS) </b><br>

<p align="center"><b>Kelompok 1</b><br>
 Annisa Kartika Utami 			(1603061)<br>
 Ari Irawan			(1603063)<br>
 Hasri Habbeana Pertiwi			(1603070)<br>
 Imam Muhayat    	(1603071)<br>
 Ade Kartono    	(1503029)<br><br><br>

<p align="center"><b>Jurusan Teknik Informatika</b><br>
<p align="center"><b>Politeknik Negeri Indramayu</b><br>
<p align="center"><b>2018</b><br><br>
</p>
</body>
</html>



__BAB 1 PENDAHULUAN__

__1.1 Tujuan__

Dokumen ini berisi Spesifikasi Kebutuhan Perangkat Lunak (SKPL) atau Software Requirement Spesification (SRS) untuk Aplikasi penyewaan kendaraan dan rute perjalanan.Tujuan dari penulisan dokumen ini adalah untuk memberikan penjelasan mengenai perangkat lunak yang akan dibangun baik berupa gambaran umum maupun penjelasan detail dan menyeluruh.

Pengguna dari dokumen ini adalah pengembang Aplikasi penyewaan kendaraan dan rute perjalanan dari 
perangkat lunak atau personil-personil yang terlibat dalam sistem.
Dokumen ini akan digunakan sebagai bahan acuan dalam proses pengembangan dan sebagai bahan evaluasi 
pada saat proses pengembangan perangkat lunak maupun di akhir pengembangannya. 
Dengan adanya dokumen SRS ini diharapkan pengembangan perangkat lunak akan lebih terarah dan lebih 
terfokus serta tidak menimbulkan ambiguitas terutama bagi pengembang perangkat lunak 
Aplikasi penyewaan kendaraan dan rute perjalanan.

__1.2 Lingkup__

Perangkat lunak yang akan dikembangkan adalah perangkat lunak aplikasi penyewaan kendaraan, 
yaitu merupakan perangkat lunak yang digunakan untuk mempermudah pengguna (user)
 menyewa kendaraan dan memilih jenis kendaraan beserta mengetahui rute perjalanan.

Aplikasi penyewaan  ini dapat melakukan hal-hal berikut ini :
- Pengguna (user) dapat mudah memilih kendaraan yang akan    
  disewa

- Pengguna (user) dapat mengetahui langsung harga dari 
  kendaraan yang disewa 

- Pengguna (user) dapat mengetahui rute perjalanan yang  
  akan dituju saat diperjalanan

- Admin dapat menambah dan menghapus dari kendaraan yang 
  dipakai

__1.3 Definisi, Akronim, Singkatan__

 

| Sistem |Suatu kesatuan yang terdiri komponen atau elemen yang dihubungkan bersama untuk memudahkan aliran informasi, materi atau energi untuk mencapai suatu tujuan. |
| Aplikasi |Suatu program komputer yang dibuat untuk mengerjakan dan melaksanakan tugas khusus dari pengguna. |
| Penyewaan | Sebuah persetujuan di mana sebuah pembayaran dilakukan atas penggunaan suatu barang atau properti secara sementara oleh orang lain. Barang yang dapat disewa bermacam-macam, tarif dan lama sewa juga bermacam-macam. |

Akronim dan Singkatan :
	
- SRS = Software Requirement Spesification
- RAM = Random Akses Memori
- SKPL = Spesifikasi Kebutuhan Perangkat Lunak

__1.4 Referensi__


- https://pengertiandefinisi.com/pengertian-aplikasi-dan-sejarah-perkembangan
  aplikasi/

- IEEE std.830-1998,IEEE Recomended Practice for Software Requitment Specification

- https://hansiaditya.files.wordpress.com/2007/10/uts-rpl-final02.pdf

__1.5 Overview__

Dokumen SRS ini merupakan acuan untuk mengetahui spesifikasi kebutuhan dalam menyelesaikan proyek ini.	
Dokumen SRS ini berisi tentang deskripsi kebutuhan perangkat lunak (tools pendukung , peranan sistem yang akan dikembangkan), perangkat keras, dan sumber daya manusia (SDM).
  
__BAB 2 GAMBARAN UMUM__

__2.1 Perspektif Produk__

Aplikasi Penyewaan Mobil Beserta Rute Kendaraan Alika Express ini merupakan aplikasi berbasis android yang dapat memudahkan penyewa dalam melakukan proses penyewaan kendaraan.

__2.1.1 Antarmuka Sistem__

* Use Case Costumers

![Use Case Costumers](http://i66.tinypic.com/mhbtd5.jpg)

* Use Case Admin

![Use Case Admin](http://i65.tinypic.com/34od4w5.jpg)

__2.1.2 Antarmuka Pengguna__

![1](http://i63.tinypic.com/mrb8ko.jpg)
![2](http://i67.tinypic.com/jzchav.jpg)

![3](http://i65.tinypic.com/2vs4zo9.jpg)
![4](http://i64.tinypic.com/2pt57ol.jpg)

![5](http://i63.tinypic.com/29zyo9h.jpg)
![6](http://i66.tinypic.com/hsryv6.jpg)

![7](http://i66.tinypic.com/1609yqe.jpg)
![8](http://i64.tinypic.com/152pdfb.jpg)

![9](http://i63.tinypic.com/dgo613.jpg)

__2.1.3 Antarmuka Perangkat Keras__

 

__2.1.5 Antarmuka Komunikasi__

Proses komunikasi dalam aplikasi ini melibatkan pengguna dengan perangkat mobile berbasis android.

__2.1.6 Batasan - Batasan Memori__

Batasan minimum meliputi RAM yang dibutuhkan agar sistem berjalan dengan baik adalah minimal 4 GB
sedangkan ruang cakra padat (hard disk) yang diperlukan adalah 500 GB.

__2.1.7 Operasi - Operasi__

Sebagai penyesuaian operasional untuk pengguna akan dilakukan Training bertingkat.
Tingkat user/Operator dan Supervisor, masing-masing tingkat memiliki tingkat pengetahuan yang berbeda dan hak akses sistem yang berbeda sehingga pelatihannya pun akan berberda.

__2.1.8 Kebutuhan - Kebutuhan dalam tahapan adaptasi__

* Perangkat lunak menggunakan bahasa indonesia
* Panduan aplikasi menggunakan mode interaktif
* Aplikasi ini menggunakan rute perjalanan

__2.2 Fungsi-fungsi produk__

Fungsi dari aplikasi rental mobiil berdasarkan pengguna sistem ini adalah sebagai berikut:
a. Membuat user dalam dalam membuat atau membagi sebuah atau beberapa kelompok secara acak dengan mudah dan cepat
b. Program ini bisa menginputkan list nama peminjam kemudian ditampilkan
  
 __2.3 Karakteristik pengguna__
 
Karakteristik pengguna dari perangkat lunak adalah pengguna langsung berinteraksi langsung.

__2.4 Batasan-batasan__

   Penginputan data atau memasukan nama pada aplikasi ini.
   Perangkat lunak bisa diakses ketika terhubung dengan internet 
    
__2.5 Asumsi-asumsi dan ketergantungan/keterkaitan__

   Waktu pengembangan perangkat lunak yang singkat membuat adanya kemungkinan tidak semua fungsi yang ada dapat dilaksanakan
   Pengembangan perangkat lunak tidak akan merubah file-file atau pun database yang ada
   
   
   
   
   
__2.6 Kebutuhan-kebutuhan penyeimbang__

Kebutuhan fungsional adalah kebutuhan yang harus dipenuhi agar suatu sistem dapat berjalan atau dapat dikatakan kebutuhan tambahan yang memiliki input,proses, dan output.

kebutuhan fungsional yang harus ada dalam sistem yang akan dikembangkan adalah

sebagai berikut:

1. Sistem harus dapat mempermudah pengguna/user dalam konsumen.
2. Sistem harus dapat mempermudah pengguna/ user dalam menggunakan aplikasi ini.

Kebutuhan lain yang spesifik

1. Perawatan rutin setiap minggu
2. Full service setiap bulannya


Informasi Pendukung

  1. Internet
  2. Iklan di berbagai media sosial
  3. Pamflet


__BAB 3 DESKRIPSI RINCI KEBUTUHAN__

__3.1 Kebutuhan AntarMuka Eksternal__

Kebutuhan antarmuka eksternal pada perangkat lunak Sistem Aplikasi Penyewaan Kendaraan beserta Rute Perjalanan Alikha Ekspress mencakup kebutuhan antarmuka pemakai, antarmuka perangkat keras, dan antarmuka perangkat lunak.

__3.2 Kebutuhan Fungsional__

Kebutuhan Fungsional adalah kebutuhan yang harus dipenuhi agar suatu sistem dapat berjalan atau dapat dikatakan kebutuhan tambahan yang memiliki input, proses, dan output. Kebutuhan fungsional yang harus ada dalam sistem yang akan dikembangkan ini adalah sebagai berikut:

1.	Sistem harus dapat menyediakan informasi mengenai penyewaan kendaraan secara lebih detail, cepat dan efektif.
2.	Sistem harus dapat mempermudah user dalam proses penyewaan kendaraan.

Aktor yang ada dalam dalam lingkup sistem adalah:

__a. Admin__

Yang dilakukan adalah : Login, menyediakan fasilitas untuk penyewaan kendaraan(memasukkan stok kendaraan, memberikan promo) dan Memilih menu-menu yang tersedia.

__b. Customer__

Yang dilakukan adalah : Login , melakukan pemesanan (Mengisi data, melihat data mobil) dan Memilih menu-menu yang tersedia.

__3.3 Structur Logis dari Data__
![ERD](http://i66.tinypic.com/t86cna.jpg)

__3.4 Pemeliharaan__

Untuk pemeliharaannya dapat dilakukan oleh admin dengan cara memantau , mengupdate ataupun menghapus data kendaraan yang tersedia pada Sistem Aplikasi Penyewaan Kendaraan Beserta Rute Perjalanan (Alikha Express).
