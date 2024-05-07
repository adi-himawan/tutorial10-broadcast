## Tutorial 10 - Broadcast

#### Commit 1
![Commit 1](/img/commit1.png)

Untuk menjalankan program, saya akan membuka 4 terminal terlebih dahulu. Pada salah satu terminal, saya akan menjalankan `cargo run --bin server` untuk membuat instance server. Kemudian, pada ketiga terminal lainnya, saya akan menjalankan `cargo run --bin client` untuk membuat 3 instance client. 

Berdasarkan lampiran di atas, dapat dilihat bahwa pertama-tama server akan menerima pesan yang dikirim oleh salah satu client. Setelah itu, server akan melakukan broadcast chat atau mengirimkan pesan tersebut ke setiap client.

#### Commit 2
![Commit 2](/img/commit2.png)
Ketika kita mengubah port pada sisi client, kita secara tidak langsung memberi instruksi kepada client untuk terhubung ke server melalui port tersebut. Begitu juga sebaliknya. Oleh karena itu, client dan server harus memiliki port yang sama agar keduanya bisa saling berkomunikasi.

Jika keduanya memiliki port yang berbeda, server dapat tetap berjalan dengan normal. Sebaliknya, client akan mengalami error karena tidak menemukan koneksi ke server.