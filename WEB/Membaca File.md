WRITE UP | Membaca File
-------------------------------------
Kategori: Web

Kerentanan pada soal CTF kali ini adalah kerentanan Directory Traversal. Jenis kerentanan yang memungkinkan kita untuk mengakses file dan direktori yang seharusnya tidak dapat diakses di server web. Ini dapat dilakukan dengan menggunakan tanda ".." dalam permintaan HTTP untuk mengakses file di luar direktori yang diizinkan. Tujuan kita pada soal CTF kali ini adalah memanfaatkan kerentanan Directory Traversal untuk mendapatkan flag diluar direktori yang diizinkan.

SOLVED
------------------------------
1. Pertama kita lihat terlebih dahulu hint yang ada. Inti dari hint ini adalah soal ini berkaitan dengan Directory Traversal.
![1](https://user-images.githubusercontent.com/113501500/213712573-86431de6-0a60-4a14-9a23-9a486a5296ba.png)

2. Ini adalah halaman web yang dituju. Ada search bar untuk mencari file yang akan kita cari. Search bar itu juga yang akan kita gunakan untuk memasukkan perintah Directory Traversal. BTW GIF KUCINGNYA LUCUU WKWKWK.
![2](https://user-images.githubusercontent.com/113501500/213712469-dabecaac-9608-4a42-9b17-f7a4c0c4e32f.png)

3. Pertama kita coba masukkan perintah untuk melihat isi file flag.txt dengan mengetik `flag.txt` pada search bar dan muncul hasil bahwa ada file bernama `flag.txt` tapi bukan file itu yang kita cari. Kenapa saya tau kalau ada file bernama `flag.txt`? Awalnya sih iseng nyoba nyoba dan ternyata malah ketemu. Tapi rata rata nama file flag emang biasanya `flag.txt`.
![3](https://user-images.githubusercontent.com/113501500/213712480-a715aeaa-d9bd-40d4-8e81-8bf78a10da6d.png)

4. Kita coba masukkan perintah Directory Traversal dengan mengetik `../flag.txt` dan muncul peringatan `
Warning: file_get_contents(../flag.txt): Failed to open stream: No such file or directory in /var/www/html/index.php on line 11` yang menandakan tidak ada file flag.txt di sini. Disini juga kita jadi tau kalau ada 3 direktori diatas kita, jadi kita masukkan perintah `../../../flag,txt` untuk melihat file flag.txt di direktori terluar.
![4](https://user-images.githubusercontent.com/113501500/213712491-d66b21d4-fadb-402a-83dd-22db07933805.png)

5. Masukkan perintah `../../../flag,txt` untuk melihat file flag.txt di direktori terluar. Muncul isi flag dari flag.txt di direktori paling luar.
![5](https://user-images.githubusercontent.com/113501500/213712607-5501289d-8584-4ae7-9307-5d6ff80834d9.png)

flagnya adalah `STEMBACTF{d1r3ct0ry_tr4v3rs4l_1s_c00l_r1ght???}`
