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

Semua hal yang tercantum didalam dokumen ini merupakan bagian dari ruang lingkup kebutuhan pembangunan perangkat lunak yang berupa aplikasi penyewaan kendaraan berbasis android yang digunakan untuk memberikan kemudahan kepada para penyewa dalam melakukan transaksi penyewaan kendaraan di Alikha Express.

__1.3 Definisi, Akronim, Singkatan__

| Definisi, Akronim dan Singkatan | Penjelasan |
| ----------------- | --------------------------- |
| SRS/SKPL | adalah dokumen yang menggambarkan secara detail spesifikasi kebutuhan software dalam pembangunan proyek perangkat lunak Aplikasi Kasir QR Code Berbasis Android.|
| DFD | adalah suatu diagram yang menggunakan notasi-notasi untuk menggambarkan arus dari data pada suatu sistem atau menjelaskan proses kerja suatu sistem, yang penggunaannya sangat membantu untuk memahami sistem secara logika, tersruktur dan jelas.|
| Software | Perangkat Lunak.|
| Hardware | Perangkat Keras|
| SRS | Software Requirements Specification.|
| SKPL | Spesifikasi Kebutuhan Perangkat Lunak.|
| DFD | Data Flow Diagram|
| IEEE | The Institute of Electrical and Electronics Engineers|


__1.4 Referensi__


- https://pengertiandefinisi.com/pengertian-aplikasi-dan-sejarah-perkembangan
  aplikasi/

- IEEE std.830-1998,IEEE Recomended Practice for Software Requitment Specification

- https://hansiaditya.files.wordpress.com/2007/10/uts-rpl-final02.pdf

__1.5 Overview__

Dokumen SRS ini merupakan acuan untuk mengetahui spesifikasi kebutuhan dalam menyelesaikan proyek ini.	
Dokumen SRS ini berisi tentang deskripsi kebutuhan perangkat lunak (tools pendukung , peranan sistem yang akan dikembangkan), perangkat keras, dan sumber daya manusia (SDM).
  
__BAB 2 GAMBARAN UMUM__

Kendaraan merupakan salah satu kebutuhan yang tidak bisa ditinggalkan dalam keseharian, dimana pada zaman modern ini mobil menjadi primadona bagi masyarakat untuk dapat melakukan perjalanan. Bukan hanya karena kenyamanan yang ditawarkan, melainkan juga muatan yang dapat diangkut mobil jauh lebih besar. Namun dengan segala kelebihan tersebut membuat harga mobil tidaklah murah, akan tetapi banyaknya kebutuhan masyarakat akan pentingnya mobil semakin hari semakin bertambah. Karena alasan tersebut membuat banyak kalangan yang menyediakan layanan rental mobil, termasuk rental mobil Alikha Express. Dalam kasus ini Alikha Express masih menggunakan cara manual dalam melakukan transaksi penyewaan mobil. Dimana customers harus datang langsung untuk menyewa mobil, tanpa mengetahui apakah masih ada stok mobil yang tersedia.

Penggunaan smartphone berbasis android sudah sangat mengakar di kalangan masyarakat saat ini, dari berbagai usia, profesi dan latar belakang. Hal tersebut menjadi alasan banyaknya aplikasi yang telah diciptakan untuk perangkat berbasis android. Karena masalah tersebut membuat kelompok kami berinisiatif untuk membuat aplikasi penyewaan rental mobil beserta rute kendaraan Alikha Express berbasis android. Dimana pada aplikasi ini terdapat 2 user, yaitu admin dan customers.

__2.1 Perspektif Produk__

Aplikasi penyewaan mobil beserta rute perjalanan Alika Express ini merupakan aplikasi berbasis android yang dapat memudahkan customers dalam melakukan proses penyewaan mobil. Dimana user customers dapat mengakses aplikasi ini melalui sistem android dan user admin melakukan pengolahan data menggunakan sistem web.

Sistem aplikasi penyewaan yang difasilitasi bagi customers antara lain tentunya customers dapat melakukan transaksi penyewaan mobil secara online melalui smartphone masing-masing, melihat data stok mobil dan detail mobil serta dapat melihat lokasinya dengan menggunakan maps yang tersedia pada aplikasi. Customers juga harus menginputkan data diri yang valid kedalam sistem saat melakukan proses register.

Adapun admin mengelola data mobil melalui sistem web. Dimana admin dapat menambahkan, mengedit maupun menghapus data stok kendaraan dan data detail kendaraan. Admin juga dapat melihat data customers yang berasal dari data yang telah di inputkan oleh customers. Serta admin juga dapat melihat laporan dari transaksi penyewaan yang pernah dilakukan.

__2.1.1 Antarmuka Sistem__

![](http://i65.tinypic.com/10zddnm.jpg)

| Modul | Fungsi |
|-------|--------|
| Modul otorisasi | Menangani otorisasi pengguna |
| Modul kendaraan | Menangani data kendaraan |
| Modul booking | Menangani pemesanan kendaraan |
| Modul transaksi | Menangani transaksi pembayaran sewa |
| Modul denda | Menangani perhitungan pembayaran denda |
| Modul laporan | Menangani rekap keuntungan, dll |

__2.1.2 Antarmuka Pengguna__

<table>
		<tr align="center">
			<td><b>Splash Screen</b></td>
			<td><b>Login</b></td>
			<td width="300"><b>Register</b></td>
		</tr>
		<tr  valign="top" align="center">
				<td><img src="http://i68.tinypic.com/w0lvh1.jpg" width="180" height="350" /><br><p align="justify">Tampilan splash screen akan menampilkan logo dari aplikasi. Dimana splash screen ini akan mencul pada saat aplikasi baru saja dibuka.</p></td>
				<td><img src="http://i65.tinypic.com/j7evbd.jpg" width="180" height="350" /><br><p align="justify">Pada tampilan login user diarahkan untuk menginputkan username dan juga password. Terdapat juga pilihan untuk register apabila user belum memiliki akun dan pilihan ganti password apabila user lupa password.</p></td>
				<td><img src="http://i68.tinypic.com/33uewev.jpg" width="180" height="350" /><br><p align="justify">Pada register terdapat form yang yang harus diisi oleh user. Dimana data yang harus diinputka adalah data diri dari user tersebut.</p></td>		
		</tr>
		<tr align="center">
			<td><b>Transaksi Penyewaan</td>
			<td><b>List Mobil</td>
			<td><b>Detail Mobil</td>
		</tr>
		<tr valign="top" align="center">
				<td><img src="http://i66.tinypic.com/whgv9z.jpg" width="180" height="350" /><br><p align="justify">Pada tampilan transaksi penyewaan user harus menginputkan jenis mobil yang akan disewa, tanggal penyewaan, tanggal pengembalian di form yang sudah disediakan.</p></td>
				<td><img src="http://i68.tinypic.com/av3rbq.jpg" width="180" height="350" /><br><p align="justify">Pada tampilan list mobil akan menampilkan beberapa jenis mobil yang disediakan oleh Alikha Express yang digunakan untuk mempermudah user dalam memilih jenis mobil yang ingin disewa.</p></td>
				<td><img src="http://i63.tinypic.com/hs3jpg.jpg" width="180" height="350" /><br><p align="justify">Pada tampilan detail mobil maka akan tertera data detail dari mobil yang dipilih, seperti jenis mobil, nomor polisi, dll.</p></td>		
		</tr>
			</tr>
		<tr align="center">
			<td><b>Detail Pesanan</td>
			<td><b>Navigasi</td>
			<td><b>Menu Logout</td>
		</tr>
		<tr valign="top" align="center">
				<td><img src="http://i65.tinypic.com/98wv7r.jpg" width="180" height="350" /><br><p align="justify">Di tampilan detail pesanan akan menampilkan kembali data pesanan yang sebelumnya telah diinputkan oleh customers.</p></td>
				<td><img src="http://i63.tinypic.com/10o38mo.jpg" width="180" height="350" /><br><p align="justify">Navigasi ini digunakan untuk memudahkan pengguna untuk menuju menu tertentu yang tersedia di aplikasi Alikha Express.</p></td>
				<td><img src="http://i64.tinypic.com/10pn8km.jpg" width="180" height="350" /><br><p align="justify">Apabila ingin keluar dari aplikasi maka akan muncul menu pilihan logout.</p></td>		
		</tr>
		</tr>
			</tr>
	</table>
</div>

 - **Mockup Website**
	
<table align="center">
		<tr>
			<td><b>Login Admin</td>
		</tr>
		<tr align="center">
			<td><img src="http://i65.tinypic.com/1rvm2w.jpg" align="center"> <br><p align="justify">Login admin digunakan sebagai proses otorisasi admin agar dapat mengolah data pada sistem Alikha Express berbasis web.</p></td>
		</tr>
				<tr>
			<td><b> Stok Kendaraan </td>
		</tr>
		<tr align="center">
			<td><img src="http://i66.tinypic.com/b51o2f.jpg"><br><p align="justify">Pada tampilan stok kendaraan terdapat tabel dimana tercantum beberapa kendaraan yang tersedia di Alikha Express. Admin juga dapat melakukan perubahan terhadap data stok kendaraan.</p></td>
		</tr>
				<tr>
			<td><b> Data Transaksi </td>
		</tr>
		<tr align="center">
			<td><img src="http://i66.tinypic.com/wcbz7p.jpg"><br><p align="justify">Di dalam data transaksi terdapat tabel transaksi yang pernah dilakukan oleh sistem.</p></td>
		</tr>
				<tr>
			<td><b> Data Penyewa </td>
		</tr>
		<tr align="center">
			<td><img src="http://i67.tinypic.com/11imhkm.jpg"><br><p align="justify">Pada data penyewa terdapat tabel yang berisikan data penyewa yang telah diinputkan oleh customers melalui smartphone.</p></td>
		</tr>			
	</table>

__2.1.3 Antarmuka Perangkat Keras__

Kebutuhan minimum perangkat keras yang dapat digunakan oleh aplikasi ini adalah :

* Smarthpone Android<br>
Dibutuhkan sebuah smartphone dengan os Android yang untuk dapat menggunakan aplikasi Alikha Express ini untuk user customers.

* PC/Laptop<br>
Untuk admin membutuhkan PC/Laptop untuk dapat menggunakan aplikasi Alikha Express ini.

__2.1.4 Antarmuka Perangkat Lunak__

Perangkat lunak yang dibutuhkan untuk aplikasi ini yaitu :
* Android Studio
* Sublime Teks
* XAMPP
* Balsamiq Mockup


__2.1.5 Antarmuka Komunikasi__

Proses komunikasi dalam aplikasi ini melibatkan pengguna dengan internet.

__2.1.6 Batasan - Batasan Memori__

Batasan minimum meliputi RAM yang dibutuhkan agar sistem berjalan dengan baik adalah minimal 4 GB
sedangkan ruang cakra padat (hard disk) yang diperlukan adalah 500 GB.

__2.1.7 Operasi - Operasi__

Sebagai penyesuaian operasional untuk pengguna akan dilakukan Training bertingkat.
Tingkat user/Operator dan Supervisor, masing-masing tingkat memiliki tingkat pengetahuan yang berbeda dan hak akses sistem yang berbeda sehingga pelatihannya pun akan berberda.

__2.1.8 Kebutuhan - Kebutuhan Dalam Tahapan Adaptasi__

* Perangkat lunak menggunakan bahasa indonesia
* Panduan aplikasi menggunakan mode interaktif
* Aplikasi ini menggunakan rute perjalanan

__2.2 Spesifikasi Kebutuhan Fungsional__

 * Mobile<br>
 ![](http://i67.tinypic.com/23m6683.jpg)
 
 * Web<br>
 ![](http://i63.tinypic.com/2e5tnaq.jpg)
 
__2.3 Spesifikasi Kebutuhan Non-Fungsional__
 
* Availability<br>
Ketersediaan aplikasi yang dapat di-update sewaktu-waktu dan dapat beroperasi terus menerus selama 24 jam per hari tanpa berhenti, karena aplikasi ini akan bersifat android-based dan web-based dan akan diakses oleh pengguna yang membutuhkan dari berbagai tempat pada waktu yang berbeda-beda.

* Security<br>
Aplikasi yang dikembangkan nantinya harus memiliki tingkat keamanan yang tinggi dimana setiap user yang masuk tidak dapat seenaknya mengubah data yang berada di dalam aplikasi ini. Aplikasi ini juga aman karena terdapat transaksi penyewaan kendaran maka faktor keamanan menjadi sangat penting.

* Usability<br>
Aplikasi ini diharapkan memudahkan user dalam penggunaannya.

* Accessibility<br>
Aplikasi bisa digunakan kapanpun dan dimanapun selama terkoneksi internet.

* Portability<br>
Aplikasi ini memberi kemudahan dalam pengaksesan sistem khususnya terkait dengan faktor waktu dan lokasi pengaksesan, serta perangkat atau teknologi yang digunakan untuk mengakses.


__2.4 Karakteristik Pengguna__

__2.5 Batasan-batasan__

* Bahasa pemrograman berbasis android yang digunakan adalah Java.
* Bahasa pemrograman berbasis web yang digunakan adalah PHP dan HTML.
* DBMS yang digunakan adalah MySQL.
    
__2.6 Asumsi-Asumsi Keterkaitan__
   
__2.7 Kebutuhan-Kebutuhan Penyeimbang__

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

__3.1 Kebutuhan Antarmuka Eksternal__

Dalam operasionalnya, aplikasi yang akan dikembangkan memerlukan adanya interaksi dengan komponen-komponen lain diluar perangkat lunak itu seperti, user sebagai seorang pengguna perangkat lunak, perangkat keras dimana perangkat lunak ini akan dijalankan, perangkat komunikasi dimana perangkat lunak ini akan saling berkomunikasi dalam jaringan internet.

__3.2 Kebutuhan Fungsional__

Kebutuhan Fungsional adalah kebutuhan yang harus dipenuhi agar suatu sistem dapat berjalan atau dapat dikatakan kebutuhan tambahan yang memiliki input, proses, dan output. Kebutuhan fungsional yang harus ada dalam sistem yang akan dikembangkan ini adalah sebagai berikut:

1.	Sistem harus dapat menyediakan informasi mengenai penyewaan kendaraan secara lebih detail, cepat dan efektif.
2.	Sistem harus dapat mempermudah user dalam proses penyewaan kendaraan.

Aktor yang ada dalam dalam lingkup sistem adalah:

__a. Admin__

Yang dilakukan adalah : Login, menyediakan fasilitas untuk penyewaan kendaraan(memasukkan stok kendaraan, memberikan promo) dan Memilih menu-menu yang tersedia.

__b. Customer__

Yang dilakukan adalah : Login , melakukan pemesanan (Mengisi data, melihat data mobil) dan Memilih menu-menu yang tersedia.

__3.3 Struktur Detail Kebutuhan Non-Fungsional__

__3.3.1 Logika Struktur Data__
![ERD](http://i66.tinypic.com/t86cna.jpg)
