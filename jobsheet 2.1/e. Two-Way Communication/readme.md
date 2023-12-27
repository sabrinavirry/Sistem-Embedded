# E. ESP-NOW | Two-Way Communication

## 1. Cek DHT11

### a. Rangkaian
Rangkaian pada percobaan ini adalah sebagai berikut

![rangkaian ](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/17fae4a5-6535-4caa-884e-29f4be293c09)


### b. Source Code
Kode program dapat dilihat <a href="https://github.com/sabrinavirry/Sistem-Embedded/blob/master/jobsheet%202.1/e.%20Two-Way%20Communication/1.%20program%20contoh%20pengecekan%20sensor%20DHT11/2_unit_ESP32_dan_2_unit_sensor_DHT11.ino">di sini</a>

### c. Hasil dan Pembahasan
Percobaan ini adalah mengecek sensor DHT11 dengan menghubungkannya ke board ESP dan menjalankan program diatas. Jika sensor berfungsi dengan baik,
pada serial monitor akan menampilkan suhu dan kelembaban yang terbaca oleh sensor.

[masukan hasil]

## 2. Two-Way Communication

### a. Rangkaian
Rangkaian pada percobaan ini adalah sebagai berikut
![rangkaian2](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/810c7382-70c9-4090-8d30-b66d99d72aaf)

![rangkaian ](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/17fae4a5-6535-4caa-884e-29f4be293c09)

### b. Source Code
Kode program dapat dilihat <a href="https://github.com/sabrinavirry/Sistem-Embedded/blob/master/jobsheet%202.1/e.%20Two-Way%20Communication/2.%20mengirim%20data%20dht11%20ke%20board%20eps32%20lain/2_unit_ESP32_dan_2_unit_sensor_DHT11_program2.ino">di sini</a>

### c. Hasil dan Pembahasan
Percobaan ini menggunakan 2 board ESP32 yang saling berkomunikasi. Hasil sensor ESP A dikirim ke ESP B dan juga sebaliknya dalam interval waktu tertentu sehingga program menggabungkan fungsi pengiriman dan penerimaan data serta pembacaan sensor sekaligus.

[masukan hasil]


