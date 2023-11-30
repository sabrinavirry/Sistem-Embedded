# B. Mengakses Sensor DHT 11 (Single Wire / BUS)

# 1. Sensor DHT 11 | A. Cek Sensor DHT11

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
![Rangkaian ](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/7d8be0fe-bd30-4938-8a42-1534f868108b)


## 3. Hasil dan Pembahasan
Dari hasil praktikum ini kita dapat mengerti cara mengecek Sensor DHT 11, dimana setelah mengecek kita dapat mengetahui jika sensor berfungsi dengan baik maka serial monitor akan menampilkan hasil  suhu dan kelembaban  sensor DHT11.

### Hasil Percobaan



### Source Code
Program dapat dilihat <a href="https://github.com/sabrinavirry/Sistem-Embedded/blob/master/jobsheet%202/a.%20EP32%20Capacitive%20Touch%20Sensor/1.%20program%20contoh%20touch%20test/touch_1.ino"> disini </a> atau dibawah ini
![Program contoh touch](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/a7fa7af9-3a41-4f59-b262-d289d74a95a7)

## 4. Kesimpulan

Dari praktikum ini, kita dapat mengetahui bahwa kita bisa mengetahui cara kerja dari sensor DHT 11().

<br></br>
# 2. Sensor DHT 11 | Studi Kasus

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

![Jobsheet Embedded](https://github.com/brianrahma/brian-system-embedded/assets/82065700/644f9625-2d44-451c-9cf8-ce842129bb98)

## 3. Hasil dan Pembahasan
Dalam praktikum ini hasil dari tugas ini adalah ketika sensor mendeteksi peningkatan suhu. Apabila suhu dibawah 30 derajat, ESP32 akan mematikan buzzer dan menyalakan LED berbentuk running LED. dan sedangkan suhu monitor serial juga meningkat.  Saat suhu ruangan mencapai 30 derajat Celcius, ESP32  menyalakan LED merah dan buzzer. 

### Hasil Percobaan

### Source Code

Program dapat dilihat <a href="https://github.com/sabrinavirry/Sistem-Embedded/blob/master/jobsheet%202/a.%20EP32%20Capacitive%20Touch%20Sensor/2.%20LED%20menyala%20ketika%20sensor%20disentuh%2C%20dan%20LED%20akan%20mati%20ketika%20sensor%20tidak%20disentuh/touch_2.ino"> disini </a> atau dibawah ini
![LED menyala ketika sensor disentuh](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/c6c95bb7-e30f-444d-8647-563d43122433)

## 4. Kesimpulan

Praktikum ini kita dapat mengetahui ketika sensor mendeteksi peningkatan suhu, saat suhu ruangan mencapai 30 derajat Celcius maupun pada saat tidak mencapai suhu tersebut.

<br><br>
