# D. ESP-NOW | One-Way, Many-to-One Communication

## One-Way, Many-to-One Communication

### a. Rangkaian
Rangkaian pada percobaan ini adalah sebagai berikut
![rangkaian](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/9da09db0-fd2e-4636-87bc-bdc1e6393c3b)



### b. Source Code
Pada percobaan ini, kelompok kami sebagai Slave (receiver) <br>
Kode program dapat dilihat <a href="https://github.com/sabrinavirry/Sistem-Embedded/blob/master/jobsheet%202.1/d.%20One-Way,%20Many-to-One%20Communication/1.%203%20board%20diatur%20sebagai%20Sender%20dan%201%20board%20diatur%20sebagai%20receiver/receiver.ino">di sini</a>

### c. Hasil dan Pembahasan
Pada percobaan ini, "One" mengacu pada perangkat penerima tunggal, dan "Many" merujuk pada banyak perangkat pengirim. Ini berarti bahwa satu perangkat penerima menerima data dari beberapa perangkat pengirim secara bersamaan atau secara bergantian, namun tidak memberikan respons atau balasan kepada perangkat pengirim. Pada percobaan ini menggunakan 1 ESP32 sebagai penerima dan 3 ESP32 sebagai pengirim.
Output yang dihasilkan adalah sebagai berikut

##### Master
masukan hasil 

##### Slave
masukan hasil

Dapat dilihat bahwa receiver mendapatkan 3 buah data dari 3 sender, dengan memperhatikan MAC Address pengirim berjumlah 3 buah

