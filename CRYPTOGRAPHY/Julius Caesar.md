WRITE UP | Julius Caesar
-------------------------------------
Kategori: CRYPTOGRAPHY

Pada CTF soal CRYPTOGRAPHY ini kita bertujuan untuk mendekrip `sandi Caesar`. `Sandi Caesar`, atau `sandi geser`, `sandi Caesar` atau `Geseran Caesar` adalah salah satu teknik `enkripsi` paling sederhana dan paling terkenal. Sandi ini termasuk sandi substitusi dimana setiap huruf pada teks terang `(plaintext)` digantikan oleh huruf lain yang memiliki selisih posisi tertentu dalam alfabet. Misalnya, jika menggunakan `geseran 3`, `W` akan menjadi `Z`, `I` menjadi `L`, dan `K` menjadi `N` sehingga teks terang `"wiki"` akan menjadi `"ZLNL"` pada teks tersandi. Nama `Caesar` diambil dari `Julius Caesar`, jenderal, konsul, dan diktator Romawi yang menggunakan sandi ini untuk berkomunikasi dengan para panglimanya.

SOLVED
------------------------------
1. Pertama baca terlebih dahulu soalnya. Pada soal CTF ini kita diberikan suatu kalimat berupa hasil `enkripsi` dari `Sandi Caesar` dengan `shift key 7`. 
![1](https://user-images.githubusercontent.com/113501500/213875560-9a307314-e58d-43b3-947e-465f72c212c7.png)

2. 
![2](https://user-images.githubusercontent.com/113501500/213875565-7994d19e-87a0-4709-81f8-c1997041e714.png)

![3](https://user-images.githubusercontent.com/113501500/213875566-abef9093-666e-43fd-ad07-f5c4035f06c1.png)

![4](https://user-images.githubusercontent.com/113501500/213875571-5ef7dc11-7cf0-4590-9e0b-380730a959a0.png)

![5](https://user-images.githubusercontent.com/113501500/213875579-95b05018-4f02-47db-95bd-4183c5935d68.png)

flagnya adalah `STEMBACTF{halo_saya_adalah_caesar!!caesar_cipher??}`
