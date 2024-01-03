# E. ESP-NOW | Two-Way Communication

## 1. Cek DHT11

### a. Rangkaian
Rangkaian pada percobaan ini adalah sebagai berikut

![rangkaian ](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/17fae4a5-6535-4caa-884e-29f4be293c09)


### b. Source Code
Program dapat dilihat dibawah ini atau dapat klik <a href="https://github.com/sabrinavirry/Sistem-Embedded/blob/master/jobsheet%202.1/e.%20Two-Way%20Communication/1.%20program%20contoh%20pengecekan%20sensor%20DHT11/2_unit_ESP32_dan_2_unit_sensor_DHT11.ino">di sini</a>
![pengecekan unit](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/7d7dc3ae-406c-4d6b-b28b-79dba4bb230f)


### c. Hasil dan Pembahasan
Percobaan ini adalah mengecek sensor DHT11 dengan menghubungkannya ke board ESP dan menjalankan program diatas. Jika sensor berfungsi dengan baik,
pada serial monitor akan menampilkan suhu dan kelembaban yang terbaca oleh sensor.

![JOB 4 E-1](https://github.com/brianrahma/system-embedded/assets/82065700/db2e7688-5518-4f1d-8db0-ad185bca5071)

<p align="justify">Pada percobaan ini dilakukan pengecekan terhadap sensor DHT11. Pengecekan ini akan memberikan data-data seperti humidity, temperature, dan heat index yang dibaca oleh sensor DHT11.

## 2. Two-Way Communication

### a. Rangkaian
Rangkaian pada percobaan ini adalah sebagai berikut
![rangkaian2](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/810c7382-70c9-4090-8d30-b66d99d72aaf)

![rangkaian ](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/17fae4a5-6535-4caa-884e-29f4be293c09)


### b. Source Code
Program dapat dilihat dibawah ini atau dapat klik <a href="https://github.com/sabrinavirry/Sistem-Embedded/blob/master/jobsheet%202.1/e.%20Two-Way%20Communication/2.%20mengirim%20data%20dht11%20ke%20board%20eps32%20lain/2_unit_ESP32_dan_2_unit_sensor_DHT11_program2.ino">di sini</a>
![data sensor dht](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/cbbfb7f2-5622-4eac-b505-ebf4e4b0f7b5)

### c. Hasil dan Pembahasan
Percobaan ini menggunakan 2 board ESP32 yang saling berkomunikasi. Hasil sensor ESP A dikirim ke ESP B dan juga sebaliknya dalam interval waktu tertentu sehingga program menggabungkan fungsi pengiriman dan penerimaan data serta pembacaan sensor sekaligus.

![JOB 4 E-1-3](https://github.com/brianrahma/system-embedded/assets/82065700/2e498984-795f-4d76-8602-56a14146f47a)

<p align="justify">Pada percobaan ini dua buah ESP32 saling berkomunikasi 2 arah, yakni saling menerima dan mengirim data. Hasil pembacaan sensor DHT11 oleh ESP32 A dikirim lalu diterima oleh ESP32 B, sebaliknya hasil pembacaan sensor DHT11 oleh ESP32 B dikirim dan diterima oleh ESP32 A. Program ini menggabunngkan fungsi pengiriman dan penerimaan data serta pembacaan sensor sekaligus.

