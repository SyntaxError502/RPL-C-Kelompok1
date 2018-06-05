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
| id_customer| Integer| 11 | Primary Key| Iya |Auto_increment| Id customer auto increment |
| email| Varchar| 40 | Tidak | Tidak | -|Email customer |
| password| Varchar| 30 | Tidak | Tidak | - |Password yang digunakan user untuk login |
| username| Varchar| 30 | Tidak | Tidak | -|username yang digunakan untuk login |
| nama| Varchar| 50 | Tidak | Tidak | -|nama customer |
| alamat| Varchar| 50 | Tidak | Tidak | -|alamat customer |
| no_telp| Integer| 12 | Tidak | Tidak | -|no telp customer |
| no_ktp| Varchar| 30 | Tidak | Tidak | -|no ktp customer |

**Tabel Kendaraan**

|Nama Field  | Jenis    |  Volume  | Laju| Primary Key| contraint integrity| Deskripsi|
|------------|----------|----------|-------------|-----------|-----------|---------------------|
| id_kendaraan| Integer| 11 | Primary Key| Iya |Auto_increment| Id kendaraan auto increment |
| merk| Varchar| 30 | Tidak | Tidak | -|merk mobil |
| tahun| integer| 11 | Tidak | Tidak | - |tahun mobil |
| nopol| Varchar| 15 | Tidak | Tidak | -|nopol mobil |
| harga/hari| Varchar| 30 | Tidak | Tidak | -|harga mobil |
| gambar| Varchar| 50 | Tidak | Tidak | -|gambar mobil |

**Tabel Denda**

|Nama Field  | Jenis    |  Volume  | Laju| Primary Key| contraint integrity| Deskripsi|
|------------|----------|----------|-------------|-----------|-----------|---------------------|
| id_denda| Integer| 11 | Primary Key| Iya |Auto_increment| Id denda auto increment |
| merk| varchar| 50 | Tidak | Tidak | -|id mobil |
| denda/jam| varchar| 50 | Tidak | Tidak | - |denda/jam bila telat mengembalikan mobil |

**Tabel Pemesanan**

|Nama Field  | Jenis    |  Volume  | Laju| Primary Key| contraint integrity| Deskripsi|
|------------|----------|----------|-------------|-----------|-----------|---------------------|
| id_pemesanan| Integer| 11 | Primary Key| Iya |Auto_increment| Id pemesanan auto increment |
| id_customer| Integer| 11 | Tidak | Tidak | -|relasi untuk menghubungkan akun customer dengan data pemesanan |
| id_kendaraan| integer| 11 | Tidak | Tidak | - |relasi untuk menghubungkan data pemesanan dengan data kendaraan |
| nama| Varchar| 50 | Tidak | Tidak | -|nama customer |
| tgl_peminjaman| date| - | Tidak | Tidak | -|tanggal peminjaman mobil |
| tgl_pengembalian| date| - | Tidak | Tidak | -|tanggal pengembaian mobil |
| merk| Varchar| 50 | Tidak | Tidak | -|merk mobil |
| total| Varchar| 40 | Tidak | Tidak | -|total harga penyewaan mobil |
| gambar| Varchar| 50 | Tidak | Tidak | -|gambar bukti pembayaran |


____2.2.1 Definisi Domain/Type____ <br>
**Data admin**

| Domain Name | Power Designer Type |
|---------|---------|
|id_admin|primary key|
|username|string|
|password|string|

**Data customer**

| Domain Name | Power Designer Type |
|---------|---------|
|id_customer|primary key|
|username|string|
|password|string
|email|string|

**Data kendaraan**

| Domain Name | Power Designer Type |
|---------|---------|
|id_kendaraan|primary key|
|merk|string|
|tahun|string
|nopol|string|
|harga/hari|string|
|gambar|string

**Data Denda**

| Domain Name | Power Designer Type |
|---------|---------|
|id_denda|primary key|
|merk|string
|denda/jam|string|

**Data Pemesanan**

| Domain Name | Power Designer Type |
|---------|---------|
|id_pemesanan|primary key|
|id_customer|foreign key|
|id_kendaraan|foreign key|
|tgl_peminjaman|string|
|tgl_pengembalian|string|
|merk|string|
|total|string|
|gambar|string|

____2.2.2 Conceptual Data Model____ <br>

____2.2.3 Physical Data Model____ <br>

____2.2.4 Daftar Tabel Aplikasi____ <br>

| Nama Tabel | Primary Key | Data Store | E/R | Deskripsi Isi |
| --------- | --------- | --------- | --------- | --------- |
| admin | id_admin |  | - | Berisi username dan password admin yang digunakan untuk login |
| customer | id_customer | D2 | - |Berisi username , password customer yang digunakan untuk login dan berisi email, nama, alamat, no_telp, no_hp yang digunakan untuk reistrasi  |
| Kendaraan | id_kendaraan | D1 | - | Berisi data kendaraan yang terdapat di penyewaan tersebut |
| denda | id_denda |  | - | Berisi data denda yang digunakan untuk mengetahui berapa denda jika terlambat mengembalikan mobil |
| pemesanan | id_pemesanan | D3 | - | Berisi data pemesaan yang digunakan untuk pemesanan mobil |

__2.3 Deskripsi Modul__ <br>

### BAB 3 Deskripsi Perancangan Rinci <br>
__3.1 Diagram Konteks__ <br>

![Context Diagram](http://i63.tinypic.com/wipqar.jpg)


____3.1.1 DFD Level 0____ <br>
![DFD Level 0](http://i66.tinypic.com/30vk5rc.jpg)

____3.1.2 DFD Level 1____ <br>


__3.2 Deskripsi Rinci Tabel__ <br>
__3.2.1 Tabel Admin__
<br>Identifikasi/Nama : Admin
<br>Deskripsi Isi : Berisi data untuk login
<br>Jenis : Tabel referensi
<br>Volume : -
<br>Laju : -
<br>Primary Key : id_admin

| Id Field | Deskripsi | Tipe & Length | Boleh NULL | Default | Keterangan |
| --------- | --------- | --------- | --------- | --------- | --------- |
| id_admin | merupakan key dari tabel admin | int | No | - | Primary key yang unik setiap user, bersifat auto increment contoh : 1 |
| username | menyatakan username admin | varchar(50) | No | - | username akan digunakan sebagai username untuk login admin |
| password | menyatakan password admin | varchar(30) | No | - | password akan digunakan untuk login admin|

__3.2.2 Tabel Customer__
<br>Identifikasi/Nama : Customer
<br>Deskripsi Isi : Berisi data untuk regitrasi dan login
<br>Jenis : Tabel referensi
<br>Volume : -
<br>Laju : -
<br>Primary Key : id_customer

| Id Field | Deskripsi | Tipe & Length | Boleh NULL | Default | Keterangan |
| --------- | --------- | --------- | --------- | --------- | --------- |
| id_customer | merupakan key dari tabel admin | int(11) | No | - | Primary key yang unik setiap user, bersifat auto increment contoh : 1 |
| username | menyatakan username customer | varchar(30) | No | - | username akan digunakan sebagai username untuk login customer |
| password | menyatakan password customer | varchar(30) | No | - | password akan digunakan untuk login customer |
| nama | menyatakan nama customer | varchar(50) | No | - | nama akan digunakan untuk registrasi |
| alamat | menyatakan alamat customer | varchar(50) | No | - | alamat akan digunakan untuk registrasi |
| no_telp | menyatakan no telp customer | integer(12) | No | - | no telp akan digunakan untuk registrasi |
| no_ktp | menyatakan no ktp customer | varchar(30) | No | - | no ktp akan digunakan untuk registrasi |
| email | menyatakan email customer | varchar(40) | No | - | email akan digunakan untuk registrasi |

__3.2.3 Tabel Kendaraan__
<br>Identifikasi/Nama : Kendaraan
<br>Deskripsi Isi : Berisi data Kendaraan
<br>Jenis : Tabel referensi
<br>Volume : -
<br>Laju : -
<br>Primary Key : id_kendaraan

| Id Field | Deskripsi | Tipe & Length | Boleh NULL | Default | Keterangan |
| --------- | --------- | --------- | --------- | --------- | --------- |
| id_kendaran | merupakan key dari tabel kendaraan | int(11) | No | - | Primary key yang unik setiap user, bersifat auto increment contoh : 1 |
| merk | menyatakan merk mobil | varchar(30) | No | - | merk mobil akan digunakan pada menu data kendaran |
| tahun | menyatakan tahun mobil | int(11) | No | - | tahun mobil akan digunakan pada menu data kendaraan |
| nopol | menyatakan nopol mobil | varchar(15) | No | - | nopol mobil akan digunakan pada menu data kendaraan |
| harga/hari | menyatakan harga sewa mobil/hari | varchar(30) | No | - | harga/hari akan digunakan pada menu data kendaraan  |
| gambar | menyatakan gambar mobil | varchar(50) | No | - | gambar mobil akan diigunakan pada menu data kendaraan |

__3.2.5 Tabel Denda__
<br>Identifikasi/Nama : Denda
<br>Deskripsi Isi : Berisi data denda
<br>Jenis : Tabel referensi
<br>Volume : -
<br>Laju : -
<br>Primary Key : id_denda

| Id Field | Deskripsi | Tipe & Length | Boleh NULL | Default | Keterangan |
| --------- | --------- | --------- | --------- | --------- | --------- |
| id_denda | merupakan key dari tabel denda | int(11) | No | - | Primary key yang unik setiap user, bersifat auto increment contoh : 1 |
| merk | menyatakan merk mobil | varchar(50) | No | - | merk mobil akan digunakan pada data denda |
| denda/jam | menyatakan total denda | varchar(50) | No | - | denda/jam akan digunakan untuk mengetahui berapa total denda  |

__3.2.6 Tabel Pemesanan__
<br>Identifikasi/Nama : Pemesanan
<br>Deskripsi Isi : Berisi data untuk melakukan pemesanan
<br>Jenis : Tabel referensi
<br>Volume : -
<br>Laju : -
<br>Primary Key : id_pemesanan

| Id Field | Deskripsi | Tipe & Length | Boleh NULL | Default | Keterangan |
| --------- | --------- | --------- | --------- | --------- | --------- |
| id_pemesanan | merupakan key dari tabel pemesanan | int(11) | No | - | Primary key yang unik setiap user, bersifat auto increment contoh : 1 |
| id_customer| merupakan foreign key pada tabel pemesanan | int(11) | No | - | foreign key relasi untuk menghubungkan tabel pemesanan dengan data customer |
| id_kendaraan | merupakan foreign key pada tabel pemesanan | int(11) | No | - | foreign key relasi untuk menghubungkan tabel pemesanan dengan data kendaraan  |
| nama | menyatakan nama customer | varchar(50) | No | - | nama akan digunakan untuk pemesanan  |
| tgl_peminjaman | menyatakan tgl peminjaman | date | No | - |  tgl peminjaman akan digunakan untuk pemesanan   |
| tgl_pengembalian | menyatakan tgl pengembalian | date | No | - | tgl pengembalian akan digunakan untuk pemesanan  |
| merk | menyatakan merk mobil | varchar(50) | No | - | merk akan digunakan untuk mengetahui jenis mobil pada saat pemesanan |
| total | menyatakan total harga sewa | varchar(40) | No | - | total akan digunakan untuk mengetahui harga total sewa mobil  |
| gambar | menyatakan total denda | varchar(50) | No | - | gambar akan digunakan untuk mengetahui bukti pembayaran |

__3.3 Deskripsi Rinci Modul__ <br>

____3.3.1 Modul____ <br>


______3.3.1.1 Fungsi Modul______ <br>

| No | Fungsi | Jenis | Tabel Terkait |
|---------|---------|---------|---------|
| 1 | Login | form entry | user |
| 2 | Register | form entry | user |

______3.3.1.2 Spesifikasi Layar Utama______ <br>

 <table width="100%" align="center">
		<tr align="center">
			<td><b>Login</b></td>
		</tr>
		<tr  valign="top" align="center">
				<td><img src="http://i66.tinypic.com/5mbds8.jpg"/></td>	
		</tr>
		<tr align="center">
			<td><b>Register</b></td>
		</tr>
		<tr  valign="top" align="center">
				<td><img src="http://i68.tinypic.com/2duf4ac.jpg"/></td>	
		</tr>
    </table>

______3.3.1.3 Spesifikasi Query______ <br>

| ID Query | Deskripsi | Ekspresi Query |
---------|---------|---------|

| QRY01 | Login | SELECT * FROM user where username= '$username' AND password='$password' |

| QRY02 | Register | INSERT INTO user (username,nama, password,alamat, no_hp,no_ktp) VALUES ('$username,'$password','$nama',
'$alamat','$no_hp','$no_ktp') |

______3.3.1.4 Spesifikasi Field Data Layar______ <br>

| Label | Field | Tabel / Query | Validasi | Keterangan |
|---------|---------|---------|---------|---------|
| namaAdmin | nama_admin | data_admin | - | - |
| alamatAdmin | alamat_admin | data_admin | - | - |
| email | email | data_admin | - | - |

______3.3.1.5 Spesifikasi Objek-objek pada Layar______ <br>

| ID Objek | Jenis | Keterangan | Platform |
|---------|---------|---------|------------|
| texUsername | input type text | isi text akan digunakan dalam proses login sebagai username | Web |
| textPassword | input type password | isi password akan di cek apakah sesuai dengan username jika iya maka login berhasil jika tidak maka login akan gagal | Web |
|btnLogin|button|Jika di klik maka akan menjalankan QRY01 untuk melakukan proses login jika berhasil maka akan masuk ke menu utama | Web |
|textusernamel|AutoCompleteTextView| isi text akan digunakan dalam proses login sebagai username | Android |
|textPassword|EditText| isi password akan di cek apakah sesuai dengan email jika iya maka login berhasil jika tidak maka login akan gagal | Android |
|LoginBtn| Button |Jika di klik maka akan menjalankan QRY01 untuk melakukan proses login jika berhasil maka akan masuk ke menu utama | Android |
|btn_register|Button|Jika diklik maka akan menampilkan fragmen menu sign up| Android |
|btn_login|Button|Jika diklik maka akan menampilkan fragmen menu Login| Android |


______3.3.1.6 Spesifikasi Proses/Algoritma______ <br>

<br>id_proses : login, register
<br>objek terkait : username, password, button login
<br>Event:Login

|Inisial State (IS) |
|-------------------|
|Form login masih kosong|

|Final State (FS) |
|-------------------|
|Mengahsilkan otentikasi user yang masuk ke aplikasi|

|Spesifikasi Proses/Algoritma|
|----------------------------------------------------|
|1.Buka aplikasi atau web|
|2.Inputkan username dan password|
|3.If username dan password sesuai maka akan berpindah ke halaman utama aplikasi atau web|
|Else username dan password tidak sesuai maka akan tampil pesan emai dan password tidak sesuai dan user diharapkan menginput ulang username dan password|


__3.4 Matriks Kerunutan__ <br>











