WRITE UP | Beli Flag
-------------------------------------
Kategori: WEB

Kerentanan pada soal CTF kali ini adalah kerentanan pada file upload. Kerentanan ini membuat kita dapat menjalankan skrip yang berbahaya dengan hanya mengunggahnya di web tersebut. Untuk lebih lengkapnya bisa dilihat di video youtube berikut `https://www.youtube.com/watch?v=lNyOCdOV9Os&t=678s`. Tujuan CTF kali ini adalah kita mendapatkan flag yang ada di direktori shell web dengan cara mengunggah skrip yang berisikan perintah menjalankan shell untuk mendapatkan flagnya.

SOLVED
------------------------------

1. Disini ada hint berupa video di youtube. Silahkan tonton terlebih dahulu agar lebih paham dengan konsep soal CTF ini.

![1](https://user-images.githubusercontent.com/113501500/213693197-1a935e34-7dff-4dce-bc57-be0dbf85a79b.png)

2. Ini adalah tampilan webnya. Walau disini kita disuruh mengunggah file berupa gambar, namun disini saya akan mengunggah file berekstensi php. 

![3](https://user-images.githubusercontent.com/113501500/213693711-0106917f-49f8-4c6b-a463-7760e167d127.png)

3. Kita lanjut pada proses pembuatan skripnya. Silahkan buat skrip seperti dibawah ini dengan ekstensi file .php ya. Berikut ini beberapa fungsi dari sintaks pada skrip dibawah ini:
- `echo` = Sebuah perintah built-in di PHP untuk menampilkan suatu teks atau nilai variabel ke layar.
- `shell_exec` = Sebuah fungsi yang digunakan untuk mengeksekusi perintah shell dari PHP dan mengembalikan hasil dari perintah menjadi string.
- `"ls -la \"` = Perintah ini akan menampilkan daftar file dan direktori dalam direktori root "\" termasuk tanggal, waktu, ukuran file, group, dan sebagainya.

Jadi jika `echo` dan `shell_exec` digabung maka `echo` digunakan untuk menampilkan hasil yang di return oleh `shell_exec` yang merupakan hasil dari perintah shell yang dijalankan.  

![4](https://user-images.githubusercontent.com/113501500/213694856-fd878477-3531-48ae-ab63-f8429c588a42.png)

4. Pilih file skrip PHP tadi yang telah kita buat. kosongkan kolom `Filter` agar dapat memilih file selain file gambar.

![5](https://user-images.githubusercontent.com/113501500/213697319-f1018c59-9e0d-49e3-b1a0-9fdec0118fa4.png)

5. Setelah memilih file skripnya, tekan `open`.

![6](https://user-images.githubusercontent.com/113501500/213698364-f739a205-1263-4a99-8e46-fe3794fa3621.png)

6. Setelah itu tekan `Submit` dan akan muncul link PHP dibawah tombol submit. Tekan link tersebut untuk melihat hasil dari skrip yang kita buat.

![7](https://user-images.githubusercontent.com/113501500/213698580-8b8cc80b-db73-4b84-87f7-0f52987602c2.png)

7. Muncul isi direktori pada direktori root `\`. Disini juga terlihat ada file bernama `flag.txt`, bagaimana cara melihat file nya? Kita gunakan perintah `cat`.

![8](https://user-images.githubusercontent.com/113501500/213699047-b880acda-8368-4963-99de-37c4c7ad1dd7.png)

8. Berpindah ke teks editor lagi, kita ubah perintah `"ls -la \"` menjadi `"cat \flag.txt"`. Perintah ini berfungsi untuk mengeluarkan atau menampilkan isi dari file flag.txt.

![9](https://user-images.githubusercontent.com/113501500/213699087-e7671865-51b5-4f8f-b53a-a9f327e2f5cc.png)

9. Sama seperti langkah sebelumnya, kita pilih file PHP yang tadi sudah kita ganti untuk menampilkan isi file `flag.txt`.
![11](https://user-images.githubusercontent.com/113501500/213699195-24bb8f19-d344-4d36-920c-93a0d6730d68.png)

10. Kita buka link PHP yang ada di bawah. 
![12](https://user-images.githubusercontent.com/113501500/213699230-d3cf25b1-5fff-40f5-837f-32d1afc7d808.png)

11. Muncul flag hasil dari file `flag.txt`.
![13](https://user-images.githubusercontent.com/113501500/213699274-75543c5d-6302-4a22-87b8-242c9c2e4703.png)

flagnya adalah `STEMBACTF{hallo_mate_w31l_y0u_g0t_th3_f14g}`
