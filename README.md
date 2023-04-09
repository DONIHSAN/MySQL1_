# Tugas Praktikum { Pertemuan ke 5 } <img src=https://qph.fs.quoracdn.net/main-qimg-648763cc041459725b62108f4fdf5b91 width="110px" >
|**Nama**|**NIM**|**Kelas**|**Matkul**|
|----|---|-----|------|
|Muhammad Ikhsan Fakhrudin|312210019|TI.22.A2|Basis Data|

# Soal Latihan Praktikum

**1. Buat sebuah database dengan nama latihan2**

Untuk membuat database gunakan perintah sebagai berikut :

`CREATE DATABASE [nama_database]`

`CREATE DATABASE latihan2;`

lalu, setelah kita membuat database. kita masuk kedalam database tersebut dengan perintah sebagai berikut :

`USE latihan2;`

![gambar1](screenshot/ss1.png)

**2. Buat sebuah tabel dengan nama biodata (nama, alamat) didalam database latihan2!**

Untuk membuat Tabel gunakan perintah sebagai berikut :

`CREATE TABLE nama_tabel (nama_field1 tipe _data(ukuran), nama_field2 tipe_data(ukuran), ..., nama_fieldn tipe_data(ukuran));`

`CREATE TABLE biodata (nama VACHAR (15), alamat TEXT);`

![gambar2](screenshot/ss2.png)

**3. Tambahkan sebuah kolom keterangan (varchar 15), sebagai kolom terakhir!**

Untuk menambahkan kolom terakhir yaitu dengan sering digunakan kata AFTER, contoh :

`ALTER TABLE biodata ADD COLUMN keterangan VARCHAR (15) AFTER phone;`

![gambar3](screenshot/ss3.png)

**4.Tambahkan kolom id(int 11) di awal (sebagai kolom pertama)!**

Untuk menambahkan kolom pertama yaitu dengan perintah sebagai berikut :

`ALTER TABLE biodata ADD COLUMN id int(11) FIRST; `

![gambar4](screenshot/ss4.png)

**5. Sisipkan sebuah kolom dengan nama phone (varchar 15) setelah kolom alamat!**

Untuk menambahkan kolom setelah kolom lain yaitu dengan perintah `AFTER`

![gambar5](screenshot/ss5.png)

**6. Ubah tipe data kolom id menjadi char(11)!**

Untuk mengubah type data yaitu dengan perintah sebagai berikut :

`ALTER TABLE [nama_tabel] MODIFY nama_field tipe_data_baru(ukuran);`

![gambar6](screenshot/ss6.png)

**7. Ubah nama kolom phone menjadi hp (varchar 20)!**

Untuk mengubah kolom yaitu dengan perintah sebgai berikut :

`ALTER TABLE [nama_tabel] CHANGE nama_field_lama nama_field_baru tipe_data(ukuran);`

![gambar7](screenshot/ss7.png)

**8. Tambahkan kolom email setelah kolom hp**

![gambar8](screenshot/ss8.png)

**9. Hapus kolom keterangan dari tabel!**

Untuk menghapus kolom dari tabel yaitu dengan perintah sebagai berikut :

`ALTER TABLE [nama_tabel] DROP nama_field;`

![gambar9](screenshot/ss9.png)

**10. Ganti nama tabel menjadi data_mahasiswa!**

Untuk mengganti nama tabel yaitu dengan perintah sebagai berikut :

`ALTER TABLE [nama_tabel] RENAME [nama_tabel_baru];`

![gamabr10](screenshot/ss10.png)

**11. Ganti nama field id menjadi nim!**

![gambar11](screenshot/ss11.png)

**12. Jadikan nim sebagai PRIMARY KEY!**

Untuk menambahkan index atau key, gunakan perintah sebagai berikut :

tipe index :

- PRIMARY KEY
- UNIQUE KEY
- FULLTEXT

`ALTER TABLE [nama_tabel] ADD [INDEX|PRIMARY KEY] (nama_field);`

![gambar12](screenshot/ss12.png)

**13. Jadikan kolom email sebagai UNIQUE KEY!**

Perintah nya sama seperti diatas, hanya saja diganti menjadi `UNIQUE KEY`

![gambar13](screenshot/ss13.png)

# Evaluasi Dan Pertanyaan

**Tulis semua perintah-perintah SQL percobaan di pdf praktikum 1 beserta outputnya!**

SQL DDL

**Membuat Database**

`CREATE DATABASE latihan1;`

![gambar14](screenshot/ss14.png)

**Membuat Tabel**

`CREATE TABLE siswa (nama VARCHAR (100), alamat TEXT);`

![gambar15](screenshot/ss15.png)

**Menambah Kolom**

`ALTER TABLE biodata ADD COLUMN ketengan TEXT AFTER alamat;`

Di perintah yang bapak kasih ada kesalahan yaitu di nama tabelnya. seharusnya siswa bukan biodata.

![gambar16](screenshot/ss16.png)

**Menambah kolom diawal**

`ALTER TABLE siswa ADD COLUMN id INT FIRST;`

![gambar17](screenshot/ss17.png)

**Mengubah nama kolom**

`ALTER TABLE siswa CHANGE COLUMN keterangan TO kelas;`

Diperintah ini ada kesalahan, seharusnya yang benar yaitu ini ALTER TABLE siswa CHANGE keterangan kelas TEXT;

![gambar18](screenshot/ss18.png)

**Mengubah tipe data**

`ALTER TABLE siswa MODIFY COLUMN kelas VARCHAN(10);`

![gambar19](screenshot/ss19.png)

**Menghapus kolom**

`ALTER TABLE siswa DROP COLUMN kelas;`

![gambar20](screenshot/ss20.png)

**Menambah PRIMARY KEY**

`ALTER TABLE siswa ADD PRIMARY KEY(id);`

![gambar21](screenshot/ss21.png)

**Menambah CONSTRAINT**

`ALTER TABLE siswa ADD CONSTRAINT pk_sisiwa PRIMARY KEY(id);`

Disini sebenarnya tidak bermasalah jika PRIMARY KEY nya kita hapus terlebih dahulu. Jadinya saya coba ganti `PRIMARY KEY` dengan `UNIQUE KEY.`

![gambar22](screenshot/ss22.png)

**Menghapus PRIMARY KEY**

`ALTER TABLE siswa DROP PRIMARY KEY;`

![gambar23](screenshot/ss23.png)

**Menghapus CONSTRAINT**

`ALTER TABLE siswa DROP CONSTRAINT pk_siswa;`

![gambar23](screenshot/ss23.png)

## Apa Maksud Dari INT(11) ?

- INT(11) Adalah Nama Tipe Datanya Yaitu `Integer` dan Memiliki Panjang 11 Karakter.

## Ketika Kita Melihat Struktur Tabel Dengan Perintah DESC , Ada Kolom Null yang Berisi Yes dan No. Apa Maksudnya ?

- Yaitu Untuk Menjelaskan Bahwa Pada Record yg `NO` Harus diisi , Sedangkan `YES` Boleh Tidak diisi.

### Sekian Tugas Praktikum Saya di Pertemuan kali ini. Jika Masih Ada Yang Salah Saya Mohon Maaf.

### Wassalamualaikum wr.wb. <img src=https://png.pngtree.com/png-vector/20190409/ourlarge/pngtree-bye-sticker-and-bubble-speech-comic-png-image_921534.jpg width="110px" >