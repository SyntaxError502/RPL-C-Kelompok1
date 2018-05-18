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

Kendaraan merupakan salah satu kebutuhan yang tidak bisa ditinggalkan dalam keseharian, dimana di zaman modern ini mobil menjadi primadona bagi masyarakat untuk dapat melakukan perjalanan. Bukan hanya karena kenyamanannya, melainkan juga muatan yang dapat diangkut mobil jauh lebih besar. Namun dengan segala kelebihan tersebut membuat harga mobil tidaklah murah, akan tetapi banyaknya 

__2.1 Perspektif Produk__

Aplikasi Penyewaan Mobil Beserta Rute Kendaraan Alika Express ini merupakan aplikasi berbasis android yang dapat memudahkan penyewa dalam melakukan proses penyewaan kendaraan.

__2.1.1 Antarmuka Sistem__

* Use Case Costumers

![Use Case Costumers](http://i66.tinypic.com/mhbtd5.jpg)

* Use Case Admin

![Use Case Admin](http://i65.tinypic.com/34od4w5.jpg)

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
			<td><b>Halaman Mahasiswa </td>
			<td><b>Scan QR Code</td>
			<td><b>Scan Sukses</td>
		</tr>
		<tr valign="top" align="center">
				<td><img src="http://i66.tinypic.com/whgv9z.jpg" width="180" height="350" /><br><p align="justify">Pada tampilan halaman mahasiswa terdapat beberapa informasi yang bisa dilihat yakni, absensi, presensi, dan kompensasi. Ada juga 2 tombol yakni tombol jadwal dan tombol scan</p></td>
				<td><img src="http://i68.tinypic.com/av3rbq.jpg" width="180" height="350" /><br><p align="justify">Pada tampilan scan menggunakan kamera pada device untuk memindai kode QR</p></td>
				<td><img src="http://i63.tinypic.com/hs3jpg.jpg" width="180" height="350" /><br><p align="justify">Pada Tampilan sukses akan ada keterangan bahwa sudah berhasil menscan dan ada tombol tutup untuk kembali ke halaman utama</p></td>		
		</tr>
			</tr>
		<tr align="center">
			<td><b>Halaman Dosen</td>
			<td><b>Menu Dosen</td>
			<td><b>Menu Jadwal</td>
		</tr>
		<tr valign="top" align="center">
				<td><img src="http://i65.tinypic.com/98wv7r.jpg" width="180" height="350" /><br><p align="justify">Di tampilan halaman dosen, mengunakan cardview yang ditunjang dengan 2 tombol pada tiap kontentnya yakni tombl mulai pada tiap mata kuliah dan tombol ubah jadwal mata kuliah tersebut. Ada juga tombol menu yang akan bisa digunakan untuk membuka menu</p></td>
				<td><img src="http://i63.tinypic.com/10o38mo.jpg" width="180" height="350" /><br><p align="justify">Di menu terdapat keterangan nama dan NIP dosen dan ada 2 pilihan menu yakni lihat jadwal dan lihat rekap absensi</p></td>
				<td><img src="http://i64.tinypic.com/10pn8km.jpg" width="180" height="350" /><br><p align="justify">Menu jadwal akan menampilan tombol download yang akan mengunduh file jadwal yang berupa .pdf</p></td>		
		</tr>
		</tr>
			</tr>
		<tr align="center">
			<td><b>Menu Absen</td>
			<td><b>Rubah Jadwal</td>
			<td><b>List Scan Mahasiswa</td>
		</tr>
		<tr valign="top" align="center">
				<td><img src="https://2.bp.blogspot.com/-I76d037JJTA/WpJgmncc8kI/AAAAAAAAA2c/i6ko1qfOPNcX8EcQ5xQKXxjYmNw6kMGMACLcBGAs/s1600/10.png" width="180" height="350" /><br><p align="justify">Di menu rekap absen pada dosen juga sama seperti pada menu jadwal, yakni akan mendownload sebuah file yang berupa .pdf</p></td>
				<td><img src="https://2.bp.blogspot.com/-JoE6kve1QdY/WpJgmlckFHI/AAAAAAAAA2Y/xUM3uYnVlW0_GjEQOOSR2WPaehX1LGvngCLcBGAs/s1600/11.png" width="180" height="350" /><br><p align="justify">Pada menu ubah jadwal terdapat keterangan default jadwal yang sudah ditentukan, dan ada beberapa inputan yang bisa di pilih yakni masukan tanggal baru, jam baru, dan ruangan yang baru kemudian juga ada 2 tombol untuk simpan dan batal</p></td>
				<td><img src="https://3.bp.blogspot.com/-UlctF2mEaCY/WpJgn5MD00I/AAAAAAAAA2g/qvDOy_y8DTccsT65K01Ic5tzk9QSyLiuQCLcBGAs/s1600/12.png" width="180" height="350" /><br><p align="justify">List scan Mahasiswa terdapat list yang akan menampilkan daftar mahasiswa yang berhasil scan absen.</p></td>		
		</tr>
		<tr align="center">
			<td colspan="3"> <b>Splash Screen</td>
		</tr>
		<tr align="center">
			<td colspan="3"><img src="https://4.bp.blogspot.com/-RxyKPxYZ9H0/WpJgoF3xbcI/AAAAAAAAA2k/5WN4HeFuFmI1IXMcJEyXmB9S9VBghTeQQCLcBGAs/s1600/13.png" width="180" height="350" /><br><p align="justify">Tampilan splash screen terdapat keterangan aplikasi dan logo aplikasi</p></td>
		</tr>
	</table>
</div>

 - **Mockup Website**
	
<table align="center">
		<tr>
			<td><b>Dashboard Admin</td>
		</tr>
		<tr>
			<td><img src="https://4.bp.blogspot.com/-1bDyR-xSVp4/WpJhS6HlaSI/AAAAAAAAA3g/xHucj0eSHewp2QM5E_jQu0VvHIuEHVOXgCLcBGAs/s1600/dashboard.jpg"> <br><p align="justify">Pada Dashboard admin terdapat panel-panel yang berisi beberapa informasi seperti jumlah mahasiswa, jumlah dosen, jumlah kelas, kalender dan ucapan selamat datang.</p></td>
		</tr>
				<tr>
			<td><b>Data Dosen</td>
		</tr>
		<tr>
			<td><img src="https://4.bp.blogspot.com/-oTpZC5yDDHk/WpJhS11I9YI/AAAAAAAAA3Y/RWioKmHUFooXGmOEVfnGw0bycLNehL_cACLcBGAs/s1600/data%2Bdosen.jpg"><br><p align="justify">Menu Dosen terdapat tabel list nama-nama dosen dan tombol untuk edit dosen</p></td>
		</tr>
				<tr>
			<td><b>Data Kelas</td>
		</tr>
		<tr>
			<td><img src="https://1.bp.blogspot.com/-MzMv4SlEHy8/WpJhS6EDfpI/AAAAAAAAA3c/PnDpxT8VrvgGoclq7qhKIm_s7WPnQqK0QCLcBGAs/s1600/data%2Bkelas.jpg"><br><p align="justify">Di dalam menu kelas terdapat data kelas berupa table. Di dalam table tersebut juga ada tombol untuk melihat detail kelasnya</p></td>
		</tr>
				<tr>
			<td><b>Data Mahasiswa</td>
		</tr>
		<tr>
			<td><img src="https://3.bp.blogspot.com/-cimuoYqCJ-4/WpJhUMFTVUI/AAAAAAAAA3k/Ap9VlNdPOMcIqCMIGl68GLy2zydP6BeKgCLcBGAs/s1600/data%2Bmhs.jpg"><br><p align="justify">Di menu mahasiswa terdapat Data mahasiswa perkelas berupa tabel</p></td>
		</tr>
				<tr>
			<td><b>Edit Data Dosen</td>
		</tr>
		<tr>
			<td><img src="https://3.bp.blogspot.com/-WEmRHs3XnjQ/WpJhUUdmV1I/AAAAAAAAA3o/jWVkN9LXP6oKvwc3ujwbUqTSWTdWheK2wCLcBGAs/s1600/edit%2Bdosen.jpg"><br><p align="justify">Pada edit menu data dosen terdapat tombol download tamplate dan upload file berupa .xls</p></td>
		</tr>
				<tr>
			<td><b>Edit Data Mahasiswa</td>
		</tr>
		<tr>
			<td><img src="https://4.bp.blogspot.com/-tBb_4EXiMeU/WpJhUhDY_CI/AAAAAAAAA3s/S3WODC0i_ygfANN2Zmor3-KL0PSWNZV6QCLcBGAs/s1600/edit%2Bmsahasiswa.jpg"><br><p align="justify">Pada Edit Data Mahasiswa sama seperti Edit Data Dosen yakni terdapat tombol untuk upload dan download untuk mengedit data mahasiswa</p></td>
		</tr>
				<tr>
			<td><b>Jadwal</td>
		</tr>
		<tr>
			<td><img src="https://4.bp.blogspot.com/-PAD0N1WgFUo/WpJhVPhaAzI/AAAAAAAAA3w/U1FCYgLTuC0BMPXVFO9jH96Pdl0I6uyOgCLcBGAs/s1600/jadwal.jpg"><br><p align="justify">Di dalam halaman jadwal terdapat dua tombol yaitu Lihat jadwal dan ubah jadwal.</p></td>
		</tr>
				<tr>
			<td><b>Login Admin</td>
		</tr>
		<tr>
			<td><img src="https://4.bp.blogspot.com/-S7XMnGnLohQ/WpJhVY0pGrI/AAAAAAAAA30/D2kuP-a58X03M0PZjeH8SJfAKJ8OTeDeACLcBGAs/s1600/login.jpg"><br><p align="justify">Pada halaman Login terdapat beberapa input yang harus di masukan oleh admin yakni username, password dan captcha. Dan ada juga tombol untuk login</p></td>
		</tr>
				<tr>
			<td><b>Rekap Absensi</td>
		</tr>
		<tr>
			<td><img src="https://3.bp.blogspot.com/-7lixgM4oNEY/WpenRt_q7xI/AAAAAAAAA4g/CZlq-Q39w9wxeXfRHZKBdUHHqsBgT7aGgCLcBGAs/s1600/rekap.jpg"><br><p align="justify">DI halamman rekap abesnsi admin bisa langsung mendownload hasilnya dengan menekan tombol Download</p></td>
		</tr>
				<tr>
			<td><b>Tambah Data Kelas</td>
		</tr>
		<tr>
			<td><img src="https://2.bp.blogspot.com/-GQ3V8XLRJ_g/WpJhWTWWHzI/AAAAAAAAA38/pvQl-DbHKLc-AKPV23X06ncA50fhma6PQCLcBGAs/s1600/tambah%2Bkelas.jpg"><br><p align="justify">Pada tambah kelas Admin  harus memasukan nama kelas terlebih dahulu</p></td>
		</tr>
				<tr>
			<td><b>Edit Jadwal</td>
		</tr>
		<tr>
			<td><img src="https://1.bp.blogspot.com/-6GUTyCOFLns/WpJhWvUHVsI/AAAAAAAAA4A/qQnHU3tJ0soWjCHxv4PJkCxRWQwXxZKiwCLcBGAs/s1600/ubah%2Bjadwal.jpg"><br><p align="justify">Pada Edit jadwal sama seperti pada Edit mahasiswa dan dosen yakni terdapat 2 tombol untuk download tamplate dan upload untuk mengunggah data yang sudah di edit</p></td>
		</tr>
	</table>

![1](http://i68.tinypic.com/w0lvh1.jpg)
![2](http://i65.tinypic.com/j7evbd.jpg)

![3](http://i68.tinypic.com/33uewev.jpg)
![4](http://i66.tinypic.com/whgv9z.jpg)

![5](http://i68.tinypic.com/av3rbq.jpg)
![6](http://i63.tinypic.com/hs3jpg.jpg)

![7](http://i65.tinypic.com/98wv7r.jpg)
![8](http://i63.tinypic.com/10o38mo.jpg)

![9](http://i64.tinypic.com/10pn8km.jpg)

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
