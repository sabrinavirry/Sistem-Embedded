# C. Mengakses Sensor RFID (SPI Communication)

# 1. RFID | A. Cek Sensor RFID

## 1. Keterangan Singkat (Abstrak)

Dalam percobaan ini program dibuat untuk dapat memahami bagaimana cara untuk mengecek kerja dari sensor RFID.

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
Dalam praktikum ini kita dapat mengerti cara mengecek RFID. Ketika kartu RFID  didekatkan ke pembaca RFID, kode identifikasi kartu RFID  muncul  di layar serial.

### Hasil Percobaan



### Source Code
Program dapat dilihat <a href="https://github.com/sabrinavirry/Sistem-Embedded/blob/master/jobsheet%202/c.%20Mengakses%20Sensor%20RFID%20(SPI%20Communication)/1.%20program%20contoh%20RFID/rfid_1.ino"> disini </a> atau dibawah ini
![cek RFID](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/a5a9a013-9ecb-49f9-8d79-3219afe7a1d5)



## 4. Kesimpulan

Dari praktikum ini, kita dapat mengetahui bahwa kita bisa mengetahui cara kerja dari sensor RFID (SPI Communication)().

<br></br>
# 2. RFID | Studi Kasus

## 1. Keterangan Singkat (Abstrak)

Dalam percobaan ini program dibuat agar tag RFID dapat digunakan untuk mendapatkan hak akses.

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
![RFID Servo](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/5b3258df-4ebc-49fc-a5e5-581f8bb02b37)


## 4. Kesimpulan

Dalam praktikum ini, kita dapat mengetahui cara membuat program agar Tag RFID yang terbaca sebelumnya dapat digunakan untuk hak akses.
<br><br>
