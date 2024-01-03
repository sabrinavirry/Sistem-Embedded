# D. ESP-NOW | One-Way, Many-to-One Communication

## One-Way, Many-to-One Communication

### a. Rangkaian
Rangkaian pada percobaan ini adalah sebagai berikut
![rangkaian](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/9da09db0-fd2e-4636-87bc-bdc1e6393c3b)



### b. Source Code
Pada percobaan ini, kelompok kami sebagai Slave (receiver) <br>
Program dapat dilihat dibawah ini atau dapat klik <a href="https://github.com/sabrinavirry/Sistem-Embedded/blob/master/jobsheet%202.1/d.%20One-Way,%20Many-to-One%20Communication/1.%203%20board%20diatur%20sebagai%20Sender%20dan%201%20board%20diatur%20sebagai%20receiver/receiver.ino">di sini</a>
![receiver](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/0f389e3d-caad-4180-8cb0-01fafc27e178)


### c. Hasil dan Pembahasan
Pada percobaan ini, "One" mengacu pada perangkat penerima tunggal, dan "Many" merujuk pada banyak perangkat pengirim. Ini berarti bahwa satu perangkat penerima menerima data dari beberapa perangkat pengirim secara bersamaan atau secara bergantian, namun tidak memberikan respons atau balasan kepada perangkat pengirim. Pada percobaan ini menggunakan 1 ESP32 sebagai penerima dan 3 ESP32 sebagai pengirim.
Output yang dihasilkan adalah sebagai berikut

 ![JOB 4 D-1](https://github.com/brianrahma/system-embedded/assets/82065700/fc08dd91-98f1-4ab2-ba22-5e308386dbae)

 <img src="https://github.com/brianrahma/system-embedded/assets/82065700/117f129c-4f66-4567-b4a2-86dd638d2091" width="700"><br>
 <p align="justify">Dalam percobaan ini merupakan Many-to-One Communication, kata many menandakan banyaknya pengirim dan one berarti penerima tunggal. Dalam hal ini komunikasi berupa receiver tunggal yang menerima data dari 3 sender ESP32. Dari gambar diatas dapat dilihat bahwa receiver mendapatkan 3 buah data dari 3 sender yang ditandai dengan MAC Address sender yang berbeda-beda.


