WRITE UP | Jejak si Akbar
-------------------------------------
Kategori: OSINT

Pada soal CTF kali ini memiliki unsur Steganography. `Steganography` adalah teknik untuk menyembunyikan pesan atau data dalam suatu medium, seperti gambar atau suara, dengan cara yang tidak dapat dikenali secara normal. Dalam CTF ini, `steganography` sering digunakan untuk menyembunyikan flag atau pesan rahasia dalam gambar atau audio, yang harus ditemukan oleh peserta CTF melalui analisis atau teknik khusus. Pada CTF ini, pesan rahasianya berada di dalam sebuah audio. Jadi kita harus menggunakan tool online untuk melihat `spectogram`nya.

SOLVED
------------------------------

1. Pertama, kita baca terlebih dahulu soal CTF nya karena biasanya kategori OSINT ada clue di soal nya. Setelah membaca soalnya, kita tau bahwa pada soal CTF kali berhubungan dengan audio nih.....
![1](https://user-images.githubusercontent.com/113501500/213870793-735c28ae-e18b-4773-86c4-bcc220c5a74b.png)

2. Setelah membaca soal, kita baca hint nya. Di hint ini kita diberi clue untuk menggunakan tools online untuk melihat `Spectogram` nya.
![2](https://user-images.githubusercontent.com/113501500/213870805-8a18cb9f-c611-4a9c-93f1-bbb70854da83.png)

3. Kita cari tool online`Spectrum Analyzer` untuk melihat `Spectogram` nya. Berikut ini alamat website tool online nya `https://academo.org/demos/spectrum-analyzer/`. 
![3](https://user-images.githubusercontent.com/113501500/213870809-40997585-ffe9-44e6-ac70-b45f97ed510b.png)

4. Masukkan file MP3 dengan menekan `Choose File` lalu tekan tombol play 
![4](https://user-images.githubusercontent.com/113501500/213870816-653a5706-a6b2-4043-883a-8cf967ba3f54.png)

5. Muncul sebuah link di dalam `Spectogram`nya, berikut link nya `https://youtu.be/aMeXC_F5kRg`.
![5](https://user-images.githubusercontent.com/113501500/213870836-00b635bf-4c15-42b3-845a-106d5ccca476.png)

6.  Kita akan diarahkan ke sebuah video youtube
![6](https://user-images.githubusercontent.com/113501500/213870839-d866b966-9893-4922-b42b-57edf110c65a.png)

7. Kita scroll layar sampai bagian komentar. 
![7](https://user-images.githubusercontent.com/113501500/213870842-5c4e1f7a-c374-4817-aa7c-e0965821d376.png)

8. Kita buka isi balasan komentarnya dan akan terlihat flagnya.
![8](https://user-images.githubusercontent.com/113501500/213870846-60364763-b8e3-4eae-a679-5c9f7288906f.png)

flagnya adalah `STEMBACTF{Audi0_4nd_0p3n_S0urc3_1nt3llegent}`
