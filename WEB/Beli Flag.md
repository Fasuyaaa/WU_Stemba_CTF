WRITE UP Beli Flag
-------------------------------------
Kategori: Web

Kerentanan pada soal CTF kali ini adalah kerentanan tamper data. Kerentanan tamper data adalah kerentanan yang diakibatkan karena suatu web tidak memvalidasi atau mengecek suatu value yang dikirim oleh user. Hal ini dapat mengakibatkan user dapat mengubah data yang seharusnya tidak diubah. Tujuan pada soal CTF ini adalah kita diharuskan mengubah suatu value agar mencapai syarat untuk mendapatkan suatu flag

SOLVED
------------------------------

1. Sebelum memulai, kita lihat terlebih dahulu hint yang ada. Inti dari hint ini adalah kita dapat memanfaatkan 'inspect' untuk mengubah value yang ada

![1](https://user-images.githubusercontent.com/113501500/213481685-6249fddd-490d-4ba1-afa1-5227b5b8a3aa.png)

2. Setelah membuka website dari link 'http://203.89.28.27:5001/'. Kita lakukan inspect dengan menekan 'CTRL+SHIFT+i' dan kita cari 'value' di dalam tag 'input'

![2](https://user-images.githubusercontent.com/113501500/213483186-06c4fb36-ec5b-42d2-85bc-0cc71de26104.png)

3. Ubah 'value' nya menjadi 100 atau lebih

![3](https://user-images.githubusercontent.com/113501500/213483706-d739201c-6dc5-4bab-8f35-78c7e090e82f.png)

4. Setelah 'value' nya berubah, tekan tombol 'BELI' dan flag akan muncul

![4](https://user-images.githubusercontent.com/113501500/213484377-d3298fc7-9315-4057-b3f2-d184fd5e57db.png)

flagnya adalah `STEMBACTF{1nput_f0rm_1tu_m3n4kutk4n}`
