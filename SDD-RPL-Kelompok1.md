<html>
<body><div align="center"><h1>Software Design Description</h1></div>
<p align="center"><b>Version 1.0 </b><br>
<p align="center">11 Maret 2018<br><br>
<p align="center">
<img src="http://i67.tinypic.com/mwba89.png"/>
</p>

<br><p align="center"><b> APLIKASI SISTEM PENYEWAAN KENDARAAN BESERTA RUTE PERJALANAN (ALIKHA EXPRESS) </b><br>

<p align="center"><b>Kelompok 1</b><br>
 Annisa Kartika Utami 			(1603061)<br>
 Ari Irawan				  (1603063)<br>
 Hasri Habbeana Pertiwi			(1603070)<br>
 Imam Muhayat    	(1603071)<br>
 Ade Kartono    	(1503029)<br><br><br>

<p align="center"><b>Jurusan Teknik Informatika</b><br>
<p align="center"><b>Politeknik Negeri Indramayu</b><br>
<p align="center"><b>2018</b><br><br>
</p>
</body>
</html>
<html>


__BAB 1 PENDAHULUAN__


__1.1 TUJUAN__

Tujuan pembuatan SDD (Software Design Description) ini adalah untuk menjelaskan langkah langkah desain dan proses-proses dalam pembuatan sistem aplikasi yang akan diterapkan pada Aplikasi Penyewaan Kendaraan Beserta Rute Perjalanan Alikha Express, dan juga memberi definisi kebutuhan untuk sistem, spesifikasi kebutuhan fungsional.

Dokumen perancangan ini dibuat berdasarkan spesifikasi kebutuhan Aplikasi Penyewaan Kendaraan Beserta Rute Perjalanan Alikha Express yang akan dibuat. Dalam rangka membangun aplikasi tersebut, tentunya deskripsi perancangan untuk aplikasi tersebut dibutuhkan, khususnya oleh para pengembang dan pembangun aplikasi tersebut.

Fungsi utama dari Aplikasi ini adalah membantu member untuk melakukan transaksi penyewaan kendaraan melalui smartphone, dan memudahkan admin dalam melihat rekap laporan penyewaan.

__1.2 Lingkup Masalah__ <br>

Aplikasi Penyewaan Kendaraan adalah sebuah aplikasi berbasis android yang mempermudah dalam sarana penyewaan kendaraan dan transaksi. Pengguna aplikasi ini dapat melakukan pedaftaran, sign in, melihat harga dan jenis jenis mobil , memilih mobil , melakukan penyewaan kendaraan , dan melakukan transaksi. Sistem ini dikelola oleh seorang admin yang bertugas memperbaharui jenis-jenis mobil dan data admin. <br>

__1.3 Definisi, Akronim dan Singkatan__ <br>

Definisi, Akronim dan Singkatan  | Penjelasan
----------------- | -------------
DFD  | Data Flow Diagram. Diagram yang menggambarkan aliran data
ERD  | Entity Relationship Diagram. Diagram yang menggambarkan entitas suatu objek beserta relasinya.
SKPL | Spesifikasi Kebutuhan Perangkat Lunak. Sebuah dokumen yang berisi analisis terhadap suatu perangkat lunak yang akan dibangun yang dijabarkan dalam suatu spesifikasi kebutuhan.
User | Pengguna Aplikasi
Admin | Pengelola Sistem  Aplikasi.


__1.4 Aturan Penamaan dan Penomoran__ <br>

__1.5 Referensi__ <br>
Dokumen ini memiliki beberapa referensi dalam pembuatannya, yaitu sebagai berikut: <br>
<ul> <li>IEEE. 1998. IEEE Recommended Practice for Software Requirement Specification. New York : IEEE
<li>Pressman, Roger S. 2001. Software engineering: a practitioner’s approach 5th ed. New York : McGraw-Hill Companies, Inc.</li>
<li>Dokumen Spesifikasi Kebutuhan Perangkat Lunak (SKPL) Super Monster Mall</li></ul>

__1.6 Ikhtisar Dokumen__<br>
Dokumen SDD ini dibagi menjadi tiga bagian utama. Bagian pertama berisi penjelasan tentang dokumen SDD yang mencakup tujuan pembuatan dokumen ini, lingkup masalah yang diselesaikan oleh perangkat lunak yang dikembangkan, definisi, referensi dan deskripsi umum. Bagian kedua berisi diagram dan spesifikasi kelas, komponen sistem dan arsitektur sistem dari Q-PAY yang telah dispesifikasikan pada dokumen SRS. Bagian ketiga berisi deskripsi rinci masing-masing kelas.

<br>


### BAB 2 Deksripsi Perancangan Global
__2.1 Rancangan Lingkungan Implementasi__ <br>
Aplikasi ini akan dikembangkan pada lingkungan dengan spesifikasi sebagai berikut :
-	Sistem Operasi	: Android, Windows
-	Bahasa Pemrograman	: Java, PHP, HTML
-	DBMS	: MySQL
-	Tools	: Android Studio, XAMPP, Sublime Text
__2.2 Deskripsi Data__ <br>
Deskripsi tabel-tabel yang terdapat pada database pembuatan aplikasi POS Menggunakan QR-CODE Scanner ini adalah sebagai berikut :

**Tabel Admin**

|Nama Field  | Jenis    |  Volume  | Laju| Primary Key| contraint integrity| Deskripsi|
|------------|----------|----------|-------------|-----------|-----------|---------------------|
| id_admin| Integer| 11 | Primary Key| Iya |Auto_increment| Id admin auto increment |
| username| Varchar| 50 | Tidak | Tidak | -| Email yang digunakan user untuk login |
| password| Varchar| 30 | Tidak | Tidak | - |Password yang digunakan user untuk login |

**Tabel Customer**

|Nama Field  | Jenis    |  Volume  | Laju| Primary Key| contraint integrity| Deskripsi|
|------------|----------|----------|-------------|-----------|-----------|---------------------|
| id_customer| Integer| 11 | Primary Key| Iya |Auto_increment| Id user auto increment |
| email| Varchar| 40 | Tidak | Tidak | -| Email yang digunakan user untuk login |
| password| Varchar| 30 | Tidak | Tidak | - |Password yang digunakan user untuk login |
| username| Varchar| 20 | Tidak | Tidak | -| |
| nama| Varchar| 50 | Tidak | Tidak | -| |

____2.2.1 Definisi Domain/Type____ <br>

____2.2.2 Conceptual Data Model____ <br>

____2.2.3 Physical Data Model____ <br>

____2.2.4 Daftar Tabel Aplikasi____ <br>

| Nama Tabel | Primary Key | Data Store | E/R | Deskripsi Isi |
|----|---------|------|-----|---------|
|Tabel Admin      | Id_Admin     | 
|Tabel Customer   | Id_Customer  |
|Tabel Data Mobil | Id_Mobil     |
|Tabel Promo      | id_Promo     |
|Tabel Transaksi  | Id_Transaksi |

__2.3 Deskripsi Modul__ <br>

### BAB 3 Deskripsi Perancangan Rinci <br>
__3.1 Diagram Konteks__ <br>

![Context Diagram](http://i63.tinypic.com/wipqar.jpg)


____3.1.1 DFD Level 0____ <br>
![DFD Level 0](http://i66.tinypic.com/30vk5rc.jpg)

____3.1.2 DFD Level 1____ <br>


__3.2 Deskripsi Rinci Tabel__ <br>

____3.2.1 Tabel____ <br>

__3.3 Deskripsi Rinci Modul__ <br>

____3.3.1 Modul____ <br>

______3.3.1.1 Fungsi Modul______ <br>

______3.3.1.2 Spesifikasi Layar Utama______ <br>

______3.3.1.3 Spesifikasi Query______ <br>

______3.3.1.4 Spesifikasi Field Data Layar______ <br>

______3.3.1.5 Spesifikasi Objek-objek pada Layar______ <br>

______3.3.1.6 Spesifikasi Proses/Algoritma______ <br>

__3.4 Matriks Kerunutan__ <br>











