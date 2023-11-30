# C. Mengakses Sensor RFID (SPI Communication)

# 1. RFID | A. Cek Sensor RFID

## 1. Keterangan Singkat (Abstrak)

Dalam percobaan ini program dibuat untuk dapat memahami bagaimana cara untuk memperiksa atau mengecek kerja dari sensor DHT 11.

## 2. Alat dan Bahan
1. ESP32                ==> 1 buah
2. Breadboard           ==> 1 buah
3. Kabel Jumper         ==> 1 buah
4. Sensor DHT 11, RFID  ==> 1 buah
5. LED                  ==> 5 buah
6. Push Button          ==> 3 buah
7. Servo                ==> 1 buah
8. Resistor 330 Ohm     ==> 3 buah
9. Resistor 1k Ohm      ==> 3 buah
10. Resistor 10k Ohm    ==> 3 buah


### Rangkaian
![Rangkaian](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/ea39039f-9943-4990-bec3-5044040809e7)




## 3. Hasil dan Pembahasan
Dari hasil praktikum ini kita dapat mengerti cara mengecek Sensor DHT 11, dimana setelah mengecek kita dapat mengetahui jika sensor berfungsi dengan baik maka serial monitor akan menampilkan hasil  suhu dan kelembaban  sensor DHT11.

### Hasil Percobaan



### Source Code
Program dapat dilihat <a href="https://github.com/sabrinavirry/Sistem-Embedded/blob/master/jobsheet%202/c.%20Mengakses%20Sensor%20RFID%20(SPI%20Communication)/1.%20program%20contoh%20RFID/rfid_1.ino"> disini </a> atau dibawah ini
![cek sensor](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/38b89bf3-4847-4742-8be1-b4ef9607aef1)


## 4. Kesimpulan

Dari praktikum ini, kita dapat mengetahui bahwa kita bisa mengetahui cara kerja dari sensor DHT 11().

<br></br>
# 2. RFID | Studi Kasus

## 1. Keterangan Singkat (Abstrak)

Dalam percobaan ini program dibuat untuk dapat dapat menyelesaikan apabila saat suhu ruang 30 derajat().

## 2. Alat dan Bahan
1. ESP32                ==> 1 buah
2. Breadboard           ==> 1 buah
3. Kabel Jumper         ==> 1 buah
4. Sensor DHT 11, RFID  ==> 1 buah
5. LED                  ==> 5 buah
6. Push Button          ==> 3 buah
7. Servo                ==> 1 buah
8. Resistor 330 Ohm     ==> 3 buah
9. Resistor 1k Ohm      ==> 3 buah
10. Resistor 10k Ohm    ==> 3 buah

### Rangkaian
![Rangkaian](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/45af32c8-9adb-4599-a13a-2f6efed0ba58)



## 3. Hasil dan Pembahasan
Dalam praktikum ini kita dapat mengetahui program agar Tag RFID yang terbaca sebelumya dapat digunakan untuk hak akses. Apabila Tag RFID didekatkan pada Reader, maka LED Hijau akan menyala, servo akan bergerak ke kanan (lalu kembali ke posisi semula setelah 3 detik) dan di Serial Monitor akan tertampil pesan “Akses Diterima, Silahkan Masuk”. Apabila Tag RFID tidak dikenali, maka LED Merah akan menyala, servo tidak bergerak dan di Serial Monitor akan tertampil pesan “Akses Ditolak”. Gunakan Tag RFID lain untuk mencobanya.

### Hasil Percobaan

### Source Code

Program dapat dilihat <a href="https://github.com/sabrinavirry/Sistem-Embedded/blob/master/jobsheet%202/c.%20Mengakses%20Sensor%20RFID%20(SPI%20Communication)/2.%20RFID%20dikenali%20maka%20LED%20hijau%20dan%20servo%20menyala/rfid___servo.ino"> disini </a> atau dibawah ini
![suhu ruang 30 derajat](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/d337ddd7-00ea-47f7-a29d-45dd0e05667b)

## 4. Kesimpulan

Praktikum ini kita dapat mengetahui program agar Tag RFID yang terbaca sebelumya dapat digunakan untuk hak akses. Apabila Tag RFID didekatkan pada Reader, maka LED Hijau akan menyala, servo akan bergerak ke kanan (lalu kembali ke posisi semula setelah 3 detik) dan di Serial Monitor akan tertampil pesan “Akses Diterima, Silahkan Masuk”. Apabila Tag RFID tidak dikenali, maka LED Merah akan menyala, servo tidak bergerak dan di Serial Monitor akan tertampil pesan “Akses Ditolak”. Gunakan Tag RFID lain untuk mencobanya.

<br><br>








# C. Mengakses Sensor RFID (SPI Communication)

## 1. Cek RFID

### a. Rangkaian 
<img alt="image" src="https://github.com/delimaayup/jobsheetEmbedded/assets/151798889/74a26b36-91ab-4a93-8a4d-af319da6e011">

### b. Source Code
Kode program dapat dilihat <a href="1.%20rangkaian/rfid_rangkaian/rfid_rangkaian.ino">di sini</a>

### c. Hasil dan Pembahasan
Hasil dari percobaan ini adalah ketika RFID Card didekatkan pada RFID Reader maka akan muncul code deteksi RFID Card di serial monitor

https://github.com/delimaayup/jobsheetEmbedded/assets/151798889/4cc46281-a81f-41b4-8995-0269c8951e50


## 2. Tugas

### a. Rangkaian
Rangkaian pada percobaan ini adalah sebagai berikut



### b. Source Code
Kode program dapat dilihat <a href="1.%20rangkaian/rfid_rangkaian/rfid_rangkaian.ino">di sini</a>

### c. Hasil dan Pembahasan
Hasil dari percobaan ini adalah ketika tag RFID didekatkan pada Reader, maka LED Hijau akan menyala, servo akan bergerak ke kanan (lalu kembali ke posisi semula setelah 3 detik) dan di Serial Monitor akan tertampil pesan “Akses Diterima, Silahkan Masuk”. Apabila Tag RFID tidak dikenali, maka LED Merah akan menyala, servo tidak bergerak dan di Serial Monitor akan tertampil pesan “Akses Ditolak”. 


https://github.com/delimaayup/jobsheetEmbedded/assets/151798889/f0244211-40e7-49eb-8712-df14774e2d34


