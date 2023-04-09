# Tugas Praktikum { Pertemuan ke 5 } <img src=https://blog.masterdaweb.com/wp-content/uploads/2019/08/mysql-logo-png-transparent-1024x710.png width="100px" >
|**Nama**|**NIM**|**Kelas**|**Matkul**|
|----|---|-----|------|
|Muhammad Ikhsan Fakhrudin|312210019|TI.22.A2|Basis Data|

## 1. Buat sebuah database dengan nama latihan 2

Untuk membuat database gunakan perintah sebagai berikut :

`CREATE DATABASE [nama_database]`

`CREATE DATABASE latihan2;`

lalu, setelah kita membuat database. kita masuk kedalam database tersebut dengan perintah sebagai berikut :

`USE latihan2;`

![gambar1](screenshot/ss1.png)

## 2. Buat sebuah tabel dengan nama biodata (nama, alamat) didalam database latihan2!

Untuk membuat Tabel gunakan perintah sebagai berikut :

`CREATE TABLE nama_tabel (nama_field1 tipe _data(ukuran), nama_field2 tipe_data(ukuran), ..., nama_fieldn tipe_data(ukuran));`

`CREATE TABLE biodata (nama VACHAR (15), alamat TEXT);`

![gambar2](screenshot/ss2.png)

## 3. Tambahkan sebuah kolom keterangan (varchar 15), sebagai kolom terakhir!

Untuk menambahkan kolom terakhir yaitu dengan sering digunakan kata AFTER, contoh :

`ALTER TABLE biodata ADD COLUMN keterangan VARCHAR (15) AFTER phone;`

![gambar3](screenshot/ss3.png)

## 4.Tambahkan kolom id(int 11) di awal (sebagai kolom pertama)!

Untuk menambahkan kolom pertama yaitu dengan perintah sebagai berikut :

`ALTER TABLE biodata ADD COLUMN id int(11) FIRST; `

![gambar4](screenshot/ss4.png)

## 5. Sisipkan sebuah kolom dengan nama phone (varchar 15) setelah kolom alamat!

Untuk menambahkan kolom setelah kolom lain yaitu dengan perintah `AFTER`

![gambar5](screenshot/ss5.png)