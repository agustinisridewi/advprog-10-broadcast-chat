## AdvProg Tutorial 10 Broadcast Chat
Agus Tini Sridewi / 2306276004 / ADPRO A

### 2.1 Original code of the broadcast chat
![alt text](image.png)

Cara Menjalankan Program:
1. Buka 4 terminal terpisah untuk menjalankan satu server dan tiga client secara simultan.
2. Arahkan semua terminal ke direktori project tempat kode berada (menggunakan perintah cd).
3. Di terminal pertama, jalankan perintah: `cargo run --bin server`. Ini akan menjalankan server yang bertugas menerima dan mendistribusikan pesan.
4. Di tiga terminal lainnya, jalankan masing-masing perintah: `cargo run --bin client`untuk menjalankan klien yang dapat mengirim dan menerima pesan.

Server dan klien berkomunikasi melalui koneksi TCP. Saat klien mengirim pesan, server menerimanya, mencetaknya di terminal, lalu menyiarkan pesan itu ke semua klien yang terhubung. Klien kemudian menerima pesan dari server dan menampilkannya di terminal mereka. Semua proses berjalan secara asinkron, memungkinkan pertukaran pesan real-time antar banyak klien melalui satu server pusat.