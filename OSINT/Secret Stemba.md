WRITE UP | Secret Stemba
-------------------------------------
Kategori: OSINT

Kerentanan pada soal CTF kali ini adalah kerentanan Web Archive. Kerentanan ini menyebabkan kita dapat mengakses halaman web yang telah dihapus dengan bantuan tool online yaitu `Wayback Machine`. Tujuan CTF kali ini adalah kita harus mendapatkan flag dari halaman web yang telah dihapus. 

SOLVED
------------------------------
1. Pertama, kita baca dulu soalnya terlebih dahulu siapa tau ada clue yakan....... Jadi intinya di soal ini di ceritakan bahwa ada halaman page bernama `/s3cr3t_st3mb4` yang memuat informasi rahasia namun halaman page itu telah di hapus. Bagaimana kita mencari halaman page yang hilang itu?
![1](https://user-images.githubusercontent.com/113501500/213830545-6ac39a64-e9ef-4389-aeb5-7f2f6f25ad53.png)

2. Setelah memahami soal yang ada, kita lihat hint yang ada terlebih dahulu. Di hint ini kita disuruh menggunakan tool online. Tool online yang akan kita gunakan adalah `Wayback Machine`. Berikut link nya `https://archive.org/web/`.
![2](https://user-images.githubusercontent.com/113501500/213830551-a29628a3-155a-4227-8301-e7d12935d7ed.png)

3. Ini adalah halaman awal dari `Wayback Machine`. Kita masukkan alamat url `http://203.89.28.27:7777/s3cr3t_st3mb4`. Kenapa kita memasukkan alamat url itu? Karena kita akan mencari halaman page `s3cr3t_st3mb4` pada website STEMBA CTF dengan alamat url `http://203.89.28.27:7777` maka kita menggabungan antara url website dengan halaman page yang kita cari.
![4](https://user-images.githubusercontent.com/113501500/213830569-da1487a3-53ad-49e0-b52f-1bbf2b12aec3.png)

4. Setelah tekan `BROWSE`, maka muncul kalender seperti ini. Kita tekan link bertuliskan `January, 12, 2023`. Kenapa begitu? Karenan itu adalah tanggal tercatatnya halaman page dari `s3cr3t_st3mb4`.
![5](https://user-images.githubusercontent.com/113501500/213830574-e31ee025-fb3e-4e56-a558-aeb03f431d19.png)

5. Setelah di tekan link tadi, maka kita akan diarahkan menuju halaman page `s3cr3t_st3mb4` yang telah dihapus.
![6](https://user-images.githubusercontent.com/113501500/213830586-7df04ab9-364c-42e3-8b42-9b12df27ee6b.png)




flagnya adalah `STEMBACTF{w0w_4p4k4h_k4mu_d4r1_m4s4_d3p4n_br0???}`
