# B. Mengakses Sensor DHT 11 (Single Wire / BUS)

# 1. Sensor DHT 11 | A. Cek Sensor DHT11

## 1. Keterangan Singkat (Abstrak)

Dalam percobaan ini program dibuat untuk dapat memahami bagaimana cara untuk memeriksa atau mengecek kerja dari sensor DHT 11.

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
![rangkaian dht](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/5652d042-d7f5-49df-9936-d3c632b0c1c3)


## 3. Hasil dan Pembahasan
Dari hasil praktikum ini kita dapat mengerti cara mengecek Sensor DHT 11, dimana setelah mengecek kita dapat mengetahui jika sensor berfungsi dengan baik maka serial monitor akan menampilkan hasil  suhu dan kelembaban  sensor DHT11.

### Hasil Percobaan



### Source Code
Program dapat dilihat <a href="https://github.com/sabrinavirry/Sistem-Embedded/tree/master/jobsheet%202/b.%20Mengakses%20Sensor%20DHT%2011%20(Single%20Wire%20%20BUS)/1.%20program%20contoh%20dht11"> disini </a> atau dibawah ini
![cek sensor](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/38b89bf3-4847-4742-8be1-b4ef9607aef1)


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
![rangkaian](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/81e6ab41-8a26-41bf-accc-7f17cc40bccd)

## 3. Hasil dan Pembahasan
Dalam praktikum ini hasil dari tugas ini adalah ketika sensor mendeteksi peningkatan suhu. Apabila suhu dibawah 30 derajat, ESP32 akan mematikan buzzer dan menyalakan LED berbentuk running LED. dan sedangkan suhu monitor serial juga meningkat.  Saat suhu ruangan mencapai 30 derajat Celcius, ESP32  menyalakan LED merah dan buzzer. 

### Hasil Percobaan

### Source Code

Program dapat dilihat <a href="https://github.com/sabrinavirry/Sistem-Embedded/blob/master/jobsheet%202/b.%20Mengakses%20Sensor%20DHT%2011%20(Single%20Wire%20%20BUS)/2.%20saat%20suhu%20ruang%2030%20derajat%20maka%20LED%20dan%20buzzer%20nyala/dht11_2.ino"> disini </a> atau dibawah ini
![suhu ruang 30 derajat](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/d337ddd7-00ea-47f7-a29d-45dd0e05667b)

## 4. Kesimpulan

Praktikum ini kita dapat mengetahui ketika sensor mendeteksi peningkatan suhu, saat suhu ruangan mencapai 30 derajat Celcius maupun pada saat tidak mencapai suhu tersebut.

<br><br>
