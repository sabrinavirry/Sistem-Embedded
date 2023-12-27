# E. ESP-NOW | Two-Way Communication

## 1. Cek DHT11

### a. Rangkaian
Rangkaian pada percobaan ini adalah sebagai berikut

![board-5-2](https://github.com/farhanhisyam/sistemEmbedded/assets/94108385/f1ceb29a-9b82-4e35-9525-629cdad1b36e)

### b. Source Code
Kode program dapat dilihat <a href="1/2_way_comm_1/2_way_comm_1.ino">di sini</a>

### c. Hasil dan Pembahasan
Percobaan ini adalah mengecek sensor DHT11 dengan menghubungkannya ke board ESP dan menjalankan program diatas. Jika sensor berfungsi dengan baik,
pada serial monitor akan menampilkan suhu dan kelembaban yang terbaca oleh sensor.

https://github.com/farhanhisyam/sistemEmbedded/assets/94108385/38873920-3442-49ad-aa9a-954a19844ff3

## 2. Two-Way Communication

### a. Rangkaian
Rangkaian pada percobaan ini adalah sebagai berikut

![image](https://github.com/farhanhisyam/sistemEmbedded/assets/94108385/9095a6b2-c07e-41f7-ac99-c2021b27e56f)
![board-5-2](https://github.com/farhanhisyam/sistemEmbedded/assets/94108385/f1ceb29a-9b82-4e35-9525-629cdad1b36e)

### b. Source Code
Kode program dapat dilihat <a href="2/2_way_comm_2/2_way_comm_2.ino">di sini</a>

### c. Hasil dan Pembahasan
Percobaan ini menggunakan 2 board ESP32 yang saling berkomunikasi. Hasil sensor ESP A dikirim ke ESP B dan juga sebaliknya dalam interval waktu tertentu sehingga program menggabungkan fungsi pengiriman dan penerimaan data serta pembacaan sensor sekaligus.

https://github.com/farhanhisyam/sistemEmbedded/assets/94108385/8b31eeff-7d10-449f-b844-9f20abf9a716


