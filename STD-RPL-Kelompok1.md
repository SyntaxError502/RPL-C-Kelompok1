<html>
<body><div align="center"><h3>SOFTWARE TESTING DOCUMENT</h3></div>
<p align="center"><b>Version 1.1 </b><br>
<p align="center">14 Mei 2018<br><br>
<p align="center">
<img src="http://i67.tinypic.com/mwba89.png"/>
</p>

<br><div align="center"><h3> APLIKASI SISTEM PENYEWAAN KENDARAAN BESERTA RUTE PERJALANAN (ALIKHA EXPRESS) </h3><br></div>

<p align="center"><b>Kelompok 1</b><br>
 Annisa Kartika Utami 			(1603061)<br>
 Ari Irawan				  (1603063)<br>
 Hasri Habbeana Pertiwi			(1603070)<br>
 Imam Muhayat    	(1603071)<br>
 Ade Kartono    	(1503029)<br><br><br>

<div align="center"><h3>JURUSAN TEKNIK INFORMATIKA<br>
POLITEKNIK NEGERI INDRAMAYU<br>
2018</h3><br></div>
</p>
</body>
</html>




__BAB 1 PENDAHULUAN__

__*1.1 Tujuan Pembuatan Dokumen*__<br>
Dokumen ini digunakan sebagai panduan untuk melakukan pengujian terhadap perangkat lunak Aplikasi Sistem Penyewaan Kendaraan Beserta Rute Perjalanan (Alikha Express). Dokumen ini dipakai untuk melihat kemampuan dari program yang telah dirancang agar sesuai dengan keinginan dari pengguna. Pembuatan dokumen ini ditujukan untuk menguji perangkat lunak Aplikasi Sistem Penyewaan Kendaraan Beserta Rute Perjalanan (Alikha Express) yang merupakan bagian dari tugas mata kuliah Rekayasa Perangkat Lunak.

__*1.2 Deskripsi Umum Sistem*__<br>
Perangkat lunak yang akan diuji adalah "Aplikasi Sistem Penyewaan Kendaraan Beserta Rute Perjalanan (Alikha Express)”. Perangkat lunak ini adalah perangkat lunak yang digunakan untuk transaksi penyewaan kendaraan khususnya mobil di rental mobil Alikha Express. Sistem ini diimplementasikan melalui komunikasi di media antara sesama pengguna dengan sistem.

__*1.3 Deskripsi Dokumen (Ikhtisar)*__<br>
Dalam dokumen ini berisi 3 bagian utama yaitu Pendahuluan, Identifikasi dan Rencana Pengujian, Deskripsi dan Uji Hasil.


__*1.4 Definisi dan Singkatan*__<br>

* SKPL adalah Spesifikasi Kebutuhan Perangkat Lunak, atau dalam bahasa Inggris-nya sering juga disebut sebagai Software Requirements Spesification (SRS), dan merupakan spesifikasi dari perangkat lunak yang akan dikembangkan.
* SKPL-SK.K-xxxx adalah kode yang digunakan untuk merepresentasikan kebutuhan (requirement) pada SK, dengan SK merupakan kode perangkat lunak, SK.K adalah kode fase, dan xxxx adalah digit/nomor kebutuhan (requirement).
* DFD adalah Data Flow Diagram, diagram dan notasi yang digunakan untuk menunjukkan aliran data pada perangkat lunak.
* ERD adalah Entity Relationship Diagram, diagram dan notasi yang digunakan untuk merepresentasikan struktur data statis pada perangkat lunak.
* DPPL-Akkses.K-xxxx adalah kode yang digunakan untuk mengimplementasikan perancangan pada Akkses, dengan Akkses merupakan kode perangkat lunak, Akkses. adalah kode fase, dan xxxx adalah digit/nomor perancangan.

__*1.5 Dokumen Referensi*__<br><br>


__BAB 2 LINGKUNGAN PENGUJIAN PERANGKAT LUNAK__

__*2.1 Perangkat Lunak Pengujian*__<br>
Perangkat lunak ini (Alikha Express) disajikan dengan beberapa perangkat lunak lain, yaitu :

* Sistem operasi : Windows 10
* Bahasa pemrograman : Java dan PHP
* Database : XAMPP

__*2.2 Perangkat Keras Pengujian*__<br>
Perangkat keras yang diperlukan untuk menguji aplikasi Alikha Express ini adalah satu set komputer dengan spesifikasi:

* Processor : Intel® Core i5
* Memory : 8 GB DDR4
* Harddisk 500 GB

__*2.3 Material Pengujian*__<br>
Pada program "Aplikasi Sistem Penyewaan Kendaraan Beserta Rute Perjalanan (Alikha Express)” ini seorang pengunjung web dapat melakukan transaksi penyewaan mobil secara online tanpa harus datang dan menemui admin secara langsung. Admin sendiri dapat memanipulasi data pengunjung. Pengunjung dapat langsung memesan mobil dengan syarat memasukkan data diri, data tersebut akan secara otomatis masuk kedalam database sehingga admin dapat melihat data penyewa.**

__*2.4 Sumber Daya Manusia*__<br>
Persyaratan sumber daya manusia yang akan terlibat dalam proses pengujian perangkat lunak iniadalah :

* Memahami konsep pemrograman berorientasi objek dalam bahasa PHP.
* Memahami proses pengujian perangkat lunak berorientasi objek.
* Memahami konsep pemrograman database XAMPP.

__*2.5 Prosedur Umum Pengujian*__<br>

__*BAB 3 IDENTIFIKASI DAN RENCANA PENGUJIAN*__<br>

<html>
<head>
<title>Penggunaan Tag Tabel</title>
</head>
<body>
<table border="1">
    <tr>
        <td align="center" rowspan="2"><b>Kelas Uji</td>
        <td align="center" rowspan="2"><b>Butir Uji</td>
		<td align="center" colspan="2"><b>Identifikasi
		</td>
		<td align="center" rowspan="2"><b>Tingkat Pengujian</td>
		<td align="center" rowspan="2"><b>Jenis Pengujian</td>
		<td align="center" rowspan="2"><b>Penguji</td>
    </tr>
    <tr>
        <td align="center"><b>SKPL</td>
        <td align="center"><b>DUPL</td>
    </tr>
    <tr>
        <td rowspan="3">Pengujian Login Customers</td>
        <td>Pengujian nama pengguna & sandi untuk customers</td>
        <td>SKPL-AlikhaExpress.K-0001</td>
		<td>DUPL-01</td>
		<td>Pengujian sistem</td>
		<td>Black box</td>
		<td>Ari</td>
    </tr>
    <tr>
        <td>Kebenaran nama pengguna & sandi untuk customers</td>
        <td></td>
        <td>DUPL-02</td>
		<td>Pengujian sistem</td>
		<td>Black box</td>
		<td>Ari</td>
    </tr>
<tr>
        <td>Kelengkapan form yang diisi oleh customers</td>
        <td></td>
        <td>DUPL-03</td>
		<td>Pengujian sistem</td>
		<td>Black box</td>
		<td>Ari</td>
    </tr>
</table>
</body>
</html>

__*BAB 4 DESKRIPSI DAN HASIL UJI*__<br>

<html>
<head>
</head>
<body>
<table border="1">
    <tr>
        <td align="center" ><b>Identifikasi</td>
        <td align="center"><b>Deskripsi</td>
		<td align="center"><b>Prosedur Pengujian
		</td>
		<td align="center"><b>Masukan</td>
		<td align="center"><b>Keluaran yang Diharapkan</td>
		<td align="center"><b>Kriteria Evaluasi Hasil 1</td>
		<td align="center"><b>Kriteria Evaluasi Hasil 2</td>
		<td align="center"><b>Hasil yang Didapat</td>
		<td align="center"><b>Kesimpulan</td>
    </tr>
    <tr>
        <td>DUPL-01</td>
		<td>Pengujian Login Customers</td>
        <td>Memasukkan username dan password customers pada field yang tersedia</td>
        <td>Username dan password customers. Tekan button Login</td>
		<td>Ada message box untuk keberhasilan login</td>
		<td>Apabila ada text field username atau password yang tidak diisi maka akan muncul pop-up “Kolom Tidak Boleh Kosong”. </td>
		<td>Apabila data username atau password yang dimasukkan salah maka akan muncul pop-up "Username atau Password Salah"</td>
		<td>Sukses</td>
		<td>Diterima</td>
    </tr>
</table>
</body>
</html>