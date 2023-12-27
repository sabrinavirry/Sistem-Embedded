# D. ESP-NOW | One-Way, Many-to-One Communication

## One-Way, Many-to-One Communication

### a. Rangkaian
Rangkaian pada percobaan ini adalah sebagai berikut

![image](https://github.com/farhanhisyam/sistemEmbedded/assets/94108385/07f8dc96-c9ed-4185-927b-b423b7ea2f8e)


### b. Source Code
Pada percobaan ini, kelompok kami sebagai Slave (receiver) <br>
Kode program dapat dilihat <a href="one_way_many_to_one/one_way_many_to_one.ino">di sini</a>

### c. Hasil dan Pembahasan
Pada percobaan ini, "One" mengacu pada perangkat penerima tunggal, dan "Many" merujuk pada banyak perangkat pengirim. Ini berarti bahwa satu perangkat penerima menerima data dari beberapa perangkat pengirim secara bersamaan atau secara bergantian, namun tidak memberikan respons atau balasan kepada perangkat pengirim. Pada percobaan ini menggunakan 1 ESP32 sebagai penerima dan 3 ESP32 sebagai pengirim.
Output yang dihasilkan adalah sebagai berikut

##### Master

https://github.com/farhanhisyam/sistemEmbedded/assets/94108385/d01441c7-f31b-408d-9912-9244da693556

##### Slave

https://github.com/farhanhisyam/sistemEmbedded/assets/94108385/98694786-d8c7-4975-9957-7ce9b5ddd5f1

Dapat dilihat bahwa receiver mendapatkan 3 buah data dari 3 sender, dengan memperhatikan MAC Address pengirim berjumlah 3 buah

