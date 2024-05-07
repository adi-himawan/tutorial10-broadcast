## Tutorial 10 - Broadcast

#### Commit 1
![Commit 1](/img/commit1.png)

Untuk menjalankan program, saya akan membuka 4 terminal terlebih dahulu. Pada salah satu terminal, saya akan menjalankan `cargo run --bin server` untuk membuat instance server. Kemudian, pada ketiga terminal lainnya, saya akan menjalankan `cargo run --bin client` untuk membuat 3 instance client. 

Berdasarkan lampiran di atas, dapat dilihat bahwa pertama-tama server akan menerima pesan yang dikirim oleh salah satu client. Setelah itu, server akan melakukan broadcast chat atau mengirimkan pesan tersebut ke setiap client.