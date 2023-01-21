WRITE UP | Vinegar Salad
-------------------------------------
Kategori: CRYPTOGRAPHY

Pada CTF soal CRYPTOGRAPHY ini kita bertujuan untuk mendekrip `Sandi Vigenere`. `Sandi Vigenère` sebenarnya merupakan pengembangan dari `sandi Caesar`. Pada `sandi Caesar`, setiap huruf teks terang digantikan dengan huruf lain yang memiliki perbedaan tertentu pada urutan alfabet. Misalnya pada `sandi Caesar` dengan `geseran 3`, `A` menjadi `D`, `B` menjadi `E` dan seterusnya. `Sandi Vigenère` terdiri dari beberapa `sandi Caesar` dengan nilai `geseran` yang berbeda.

SOLVED
------------------------------
1. Pertama baca terlebih dahulu soalnya. Pada soal CTF ini kita diberikan suatu kalimat berupa hasil `enkripsi` yaitu `KXGDFTUXH{psn_crgn_eugyv_mmzwrgii_vatjvv}` dari `Sandi Vigenere` dengan `key SECRET` yang kita dapat dari `secret recipe of vinegar salad`.
![1](https://user-images.githubusercontent.com/113501500/213877617-68beffb1-436c-410a-bd8b-a5afc599b29e.png)

2. Hint nya hanya berisi clue bahwa kita bisa menggunakan online tool atau python script. Tapi disini kita akan menggunakan online tool saja.
![2](https://user-images.githubusercontent.com/113501500/213877631-8325aea3-d78c-460c-b822-0b667a5078ba.png)

3. Kita buka Vigenere decoder online nya `https://www.dcode.fr/vigenere-cipher`. Masukkan hasil `enkripsi` yang ada di soal tadi ke kolom `Vigenere ciphertext` dan ubah `Knowing the Key/Password:` menjadi `SECRET`. Tekan DECRYPT.
![3](https://user-images.githubusercontent.com/113501500/213877634-8faf4580-a6aa-4a99-8073-fd0139590cd1.png)

4. Flag hasil dekripsi akan muncul di bagian kiri layar.
![4](https://user-images.githubusercontent.com/113501500/213877639-3f06459d-fc8c-4f60-aa16-95c65ec3eaf1.png)

Flagnya adalah `STEMBACTF{you_knew_about_vigenere_cipher}`.
