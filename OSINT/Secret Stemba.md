WRITE UP | Secret Stemba
-------------------------------------
Kategori: OSINT

Kerentanan pada soal CTF kali ini adalah kerentanan Web Archive. Kerentanan ini menyebabkan kita dapat mengakses halaman web yang telah dihapus dengan bantuan tool online yaitu `Wayback Machine`. Tujuan CTF kali ini adalah kita harus mendapatkan flag dari halaman web yang telah dihapus. 

SOLVED
------------------------------
1. Pertama, kita baca dulu soalnya terlebih dahulu siapa tau ada clue yakan....... Jadi intinya di soal ini di ceritakan bahwa ada halaman page bernama `/s3cr3t_st3mb4` yang memuat informasi rahasia namun halaman page itu telah di hapus. Bagaimana kita mencari halaman page yang hilang itu?
![1](https://user-images.githubusercontent.com/113501500/213830545-6ac39a64-e9ef-4389-aeb5-7f2f6f25ad53.png)

2. Setelah memahami soal yang ada, kita lihat hint yang ada terlebih dahulu. Di hint ini kita disuruh menggunakan tool online. Tool online yang akan kita gunakan adalah `Wayback Machine`. Berikut link nya `https://archive.org/web/`
![2](https://user-images.githubusercontent.com/113501500/213830551-a29628a3-155a-4227-8301-e7d12935d7ed.png)
![3](https://user-images.githubusercontent.com/113501500/213830557-f08b2ba3-aec2-47bb-9584-ee17e5b7eb9a.png)
![4](https://user-images.githubusercontent.com/113501500/213830569-da1487a3-53ad-49e0-b52f-1bbf2b12aec3.png)
![5](https://user-images.githubusercontent.com/113501500/213830574-e31ee025-fb3e-4e56-a558-aeb03f431d19.png)
![6](https://user-images.githubusercontent.com/113501500/213830586-7df04ab9-364c-42e3-8b42-9b12df27ee6b.png)




flagnya adalah `STEMBACTF{1nput_f0rm_1tu_m3n4kutk4n}`
