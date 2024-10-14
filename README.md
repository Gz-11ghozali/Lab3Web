# Lab3Web
1. Persiapan Membuat Dokumen HTML
Buat file HTML baru bernama lab3_list.html.
Struktur awal HTML terdiri dari elemen-elemen dasar seperti <!DOCTYPE html>, <html>, <head>, dan <body>.
Di dalam elemen <head>, tambahkan meta tag untuk pengaturan charset dan viewport agar halaman HTML bisa diakses di berbagai perangkat.
Pada <body>, tambahkan header dengan judul Membuat List yang akan menjadi tampilan utama pada halaman.

<!DOCTYPE html>
<html lang="en">
<head>
   <meta charset="UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <title>HTML Lanjutan</title>
</head>
<body>
   <header>
      <h1>Membuat List</h1>
   </header>
</body>
</html>

2. Membuat Ordered List
Di dalam file HTML yang sama, tambahkan kode untuk membuat Ordered List (daftar berurutan).
Ordered List menggunakan tag <ol>, dan setiap item di dalamnya menggunakan tag <li>.

<section id="order-list">
   <h2>Ordered List</h2>
   <ol>
      <li>Pemrograman Web</li>
      <li>Sistem Informasi</li>
      <li>Basis Data 2</li>
   </ol>
</section>

Penjelasan:

<ol> digunakan untuk membuat daftar berurutan.
<li> menandai item di dalam daftar, yang akan otomatis diberi nomor urut.

![Screenshot 2024-10-14 013142](https://github.com/user-attachments/assets/bd5ff0cb-a506-48d0-a2ee-76b4471e8af5)

3. Membuat Unordered List
Setelah Ordered List, tambahkan Unordered List (daftar tidak berurutan).
Unordered List menggunakan tag <ul>, dan jenis penanda (bullet) dapat diatur menggunakan atribut type.

<section id="unorder-list">
<h2>Unordered List</h2>
<ul type="square">
<li>Jaringan Komputer</li>
<li>Struktur Data</li>
<li>Algoritma &amp; Pemrograman</li>
</ul>
</section>

Penjelasan:

<ul> digunakan untuk membuat daftar tidak berurutan dengan tanda bullet.
Atribut type="square" mengubah bentuk bullet menjadi kotak.

![Screenshot 2024-10-14 013240](https://github.com/user-attachments/assets/918dc444-409f-489f-8bb8-4701d9541afe)

4. Membuat Description List
Untuk membuat Description List (daftar deskripsi), gunakan tag <dl>.
Di dalamnya, <dt> digunakan untuk judul deskripsi, dan <dd> untuk penjelasannya

<section id="description-list">
   <h2>Description List</h2>
   <dl>
      <dt>Fakultas Teknik</dt>
      <dd>Teknik Industri</dd>
      <dd>Teknik Informatika</dd>
      <dd>Teknik Lingkungan</dd>
      <dt>Fakultas Ekonomi dan Bisnis</dt>
      <dd>Akuntansi</dd>
      <dd>Manajemen</dd>
      <dd>Bisnis Digital</dd>
   </dl>
</section>

Penjelasan:

<dl> digunakan untuk membuat daftar deskripsi.
<dt> untuk judul, dan <dd> untuk rincian dari judul tersebut.
  
![Screenshot 2024-10-14 013439](https://github.com/user-attachments/assets/7e70c4e7-2240-4f8e-ad8b-f4b65f291171)

5. Membuat Tabel
Buat file baru dengan nama lab3_tabel.html untuk membuat tabel.
Gunakan tag <table>, dan atur elemen-elemen tabel seperti <thead>, <tbody>, <tr>, <th>, dan <td>.

<!DOCTYPE html>
<html lang="en">
<head>
   <meta charset="UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <title>HTML Lanjutan</title>
</head>
<body>
   <header>
      <h1>Membuat Table</h1>
   </header>
   <table border="1" cellpadding="4" cellspacing="0">
      <thead>
         <tr>
            <th>No.</th>
            <th>Fakultas</th>
            <th>Program Studi</th>
         </tr>
      </thead>
      <tbody>
         <tr>
            <td>1.</td>
            <td>Teknik</td>
            <td>Teknik Informatika</td>
         </tr>
         <tr>
            <td>2.</td>
            <td>Teknik</td>
            <td>Teknik Industri</td>
         </tr>
         <tr>
            <td>3.</td>
            <td>Teknik</td>
            <td>Teknik Lingkungan</td>
         </tr>
      </tbody>
   </table>
</body>
</html>

Penjelasan:

Atribut border digunakan untuk menambahkan garis pada tabel.
Atribut cellpadding dan cellspacing digunakan untuk mengatur jarak antara konten dan batas sel.

![Screenshot 2024-10-14 013626](https://github.com/user-attachments/assets/66a39ca0-e472-42b5-9b2b-36595beb8329)

6. Menggabungkan Sel Data
Untuk menggabungkan sel secara vertikal atau horizontal, gunakan atribut rowspan dan colspan.

<table border="1" cellpadding="6" cellspacing="0">
   <thead>
      <tr>
         <th>No.</th>
         <th>Fakultas</th>
         <th>Program Studi</th>
      </tr>
   </thead>
   <tbody>
      <tr>
         <td>1.</td>
         <td rowspan="3">Teknik</td>
         <td>Teknik Informatika</td>
      </tr>
      <tr>
         <td>2.</td>
         <td>Teknik Industri</td>
      </tr>
      <tr>
         <td>3.</td>
         <td>Teknik Lingkungan</td>
      </tr>
   </tbody>
</table>

Penjelasan:

rowspan="3" menggabungkan 3 baris untuk kolom "Teknik".

![Screenshot 2024-10-14 014319](https://github.com/user-attachments/assets/e19a2cd3-0f1a-4633-ab98-2dc70bb69fae)

7. Membuat Form
Buat file baru dengan nama lab3_form.html dan tambahkan form menggunakan tag <form>.
Gunakan elemen form seperti <input>, <textarea>, dan <fieldset>

<!DOCTYPE html>
<html lang="en">
<head>
   <meta charset="UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <title>HTML Lanjutan</title>
</head>
<body>
   <header>
      <h1>Membuat Form</h1>
   </header>
   <form action="proses.php" method="post">
      <fieldset>
         <legend>Data Pelanggan</legend>
         <p>
            <label for="nama">Nama</label>
            <input type="text" id="nama" name="nama">
         </p>
         <p>
            <label for="alamat">Alamat</label>
            <textarea id="alamat" name="alamat" cols="20" rows="3"></textarea>
         </p>
         <p>
            <label>Jenis Kelamin</label>
            <input id="jk_l" type="radio" name="kelamin" value="L" /><label for="jk_l">Laki-laki</label>
            <input id="jk_p" type="radio" name="kelamin" value="P" /><label for="jk_p">Perempuan</label>
         </p>
         <p><input type="submit" value="Login"></p>
      </fieldset>
   </form>
</body>
</html>

Penjelasan:

<fieldset> digunakan untuk mengelompokkan elemen form.
<legend> memberikan judul untuk fieldset.
<input type="text"> untuk input teks, dan <textarea> untuk input teks panjang.
  
![Screenshot 2024-10-14 014501](https://github.com/user-attachments/assets/83349762-613a-46ad-8a5b-3e2aa7942c3a)

8. Menambahkan Style pada Form
Tambahkan CSS untuk memperindah form dengan style sederhana.

<style>
   form p > label {
      display: inline-block;
      width: 100px;
   }
   form input[type="text"], form textarea {
      border: 1px solid #197a43;
   }
   form input[type="submit"] {
      border: 1px solid #197a43;
      background-color: #197a43;
      color: #ffffff;
      font-weight: bold;
      padding: 5px 15px;
   }
</style>

penjelasan:

display: inline-block; mengatur label agar sejajar dengan input.
Style pada input dan textarea digunakan untuk memperindah tampilan elemen-elemen form tersebut, seperti menambahkan border agar lebih jelas dan teratur, serta memberikan efek visual yang lebih profesional. Dengan menggunakan style ini, tampilan form menjadi lebih rapi dan menarik, sehingga pengguna lebih mudah mengisi form dengan nyaman.

![Screenshot 2024-10-14 014553](https://github.com/user-attachments/assets/96ee04c7-394f-4850-bebe-7a286b310fee)




