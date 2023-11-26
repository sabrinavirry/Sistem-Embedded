# 1. EP32 | A. Capacitive Touch Sensor

## 1. Keterangan Singkat (Abstrak)

Dalam percobaan ini program dibuat untuk dapat memahami bagaimana cara kerja protokol komunikasi yang terdapat pada ESP32 seperti UART, 12C, OneWire dan SPI dan bagaimana cara memanfaatkan tranducer sensor dan actuator untuk perangkat IoT.

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

### Hasil Percobaan
![GPIO 1-GIF](https://github.com/brianrahma/brian-system-embedded/assets/82065700/be8ecc85-1328-4597-8c8f-7caabb8c38c9)


### Source Code
Program dapat dilihat <a href="https://github.com/sabrinavirry/Sistem-Embedded/blob/master/jobsheet%202/a.%20EP32%20Capacitive%20Touch%20Sensor/1.%20program%20contoh%20touch%20test/touch_1.ino"> disini </a> atau dibawah ini
![Program contoh touch](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/a7fa7af9-3a41-4f59-b262-d289d74a95a7)

## 4. Kesimpulan

Dari praktikum ini, kita dapat mengetahui bahwa kita bisa mengatur LED dengan interval waktu tertentu menggunakan perintah delay().

<br></br>
# 2. EP32 | LED menyala ketika Sensor disentuh

## 1. Keterangan Singkat (Abstrak)

Dalam percobaan ini program dibuat untuk dapat menghasilkan LED akan memberikan respon menyala apabila sensor disentuh().

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

### Hasil Percobaan

![GPIO 2-GIF](https://github.com/brianrahma/brian-system-embedded/assets/82065700/145bb445-7a7d-4b10-b7a7-170582e4cc8b)

### Source Code

Program dapat dilihat <a href="https://github.com/sabrinavirry/Sistem-Embedded/blob/master/jobsheet%202/a.%20EP32%20Capacitive%20Touch%20Sensor/2.%20LED%20menyala%20ketika%20sensor%20disentuh%2C%20dan%20LED%20akan%20mati%20ketika%20sensor%20tidak%20disentuh/touch_2.ino"> disini </a> atau dibawah ini
![LED menyala ketika sensor disentuh](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/c6c95bb7-e30f-444d-8647-563d43122433)

## 4. Kesimpulan

Program Blink LED menggunakan millis() membuat LED berkedip dengan interval waktu tertentu tanpa menggunakan delay(). Dengan memanfaatkan millis(), program tetap responsif terhadap tugas lainnya tanpa harus menunggu dan fleksibilitas dalam mengatur waktu dan keadaan LED.
<br></br>

# 3. EP32 | Ketika sensor disentuh maka LED Blink akan menyala

## 1. Keterangan Singkat (Abstrak)

Dalam percobaan ini program dibuat untuk dapat mengendalikan led menggunakan push button, dimana saat push button ditekan maka LED akan menyala.

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

### Hasil Percobaaan

![GPIO 3-GIF](https://github.com/brianrahma/brian-system-embedded/assets/82065700/d0eeafb4-a275-4a0d-aa58-a3b2638cb83e)

### Source Code

Program dapat dilihat <a href="https://github.com/sabrinavirry/Sistem-Embedded/blob/master/jobsheet%202/a.%20EP32%20Capacitive%20Touch%20Sensor/3.%20ketika%20sensor%20disentuh%2C%20LED%20menyala%20Blink/touch_3.ino"> disini </a> atau dibawah ini
![Sensor disentuh, LED Blink menyala](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/58c30ecc-3956-4c74-baf2-fbbc00b837d9)

## 4. Kesimpulan

Jika push button ditekan, LED akan menyala, dan jika tidak, LED akan mati. Nilai status push button ditampilkan di serial monitor. Jadi program ini memberikan gambaran terhadap keadaan push button dengan memanfaatkan kontrol digital pada pin-input dan pin-output mikrokontroler.

<br></br>
# 4. EP32 | LED menyala Serial Monitor menampilkan angka yang akan bertambah setiap kali sensor disentuh

## 1. Keterangan Singkat (Abstrak)

Dalam percobaan ini program dibuat untuk dapat mengendalikan led menggunakan push button, dimana saat push button kedua ditekan maka LED akan melakukan blink 500 ms sekali.

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

![280174754-389106d1-e4a8-41c3-8bed-ea941e62d3db](https://github.com/brianrahma/brian-system-embedded/assets/82065700/44dc01bb-f4f2-4a04-a194-9135b80f85e2)

## 3. Hasil dan Pembahasan

### Hasil Percobaan 

![GPIO 4-GIFF](https://github.com/brianrahma/brian-system-embedded/assets/82065700/94d70ec7-44b6-46d9-a153-fee747d457fd)

### Source Code

Program dapat dilihat <a href="https://github.com/sabrinavirry/Sistem-Embedded/blob/master/jobsheet%202/a.%20EP32%20Capacitive%20Touch%20Sensor/4.%20ketika%20LED%20menyala%20Serial%20Monitor%20menampilkan%20angka%20yang%20akan%20bertambah%20setiap%20kali%20sensor%20disentuh/touch_4.ino"> disini </a> atau dibawah ini
![LED menyala Serial Monitor menampilkan angka yang akan bertambah setiap kali sensor disentuh](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/143daddd-db19-40c0-a695-77d3cc0cf1e1)

## 4. Kesimpulan

Jika push button pertama ditekan, LED pertama akan menyala atau mati, kemudian saat push button kedua ditekan, akan membuat LED kedua berkedip dengan interval 500 ms. Percobaan ini memberikan gambaran terhadap dua LED sesuai dengan kondisi dua push button yang berbeda.

<br></br>
# 5. EP32 | LED nyala running saat sensor disentuh

## 1. Keterangan Singkat (Abstrak)

Dalam percobaan ini program dibuat untuk dapat mengendalikan led menggunakan push button, dimana saat push button ketiga ditekan maka LED akan menyala menjadi running led (menyala bergantian dari kiri ke kanan).

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

![280177873-81dfe4c2-b0fe-4576-8de2-ab5ee3ced849](https://github.com/brianrahma/brian-system-embedded/assets/82065700/f2f7564e-75b6-4791-ab99-6bae22467d27)

## 3. Hasil dan Pembahasan

### Hasil Percobaan

![GPIO 5-GIF](https://github.com/brianrahma/brian-system-embedded/assets/82065700/a1c97368-8842-4661-a74e-417e13b1c1f2)

### Sorce Code

Program dapat dilihat <a href="https://github.com/sabrinavirry/Sistem-Embedded/blob/master/jobsheet%202/a.%20EP32%20Capacitive%20Touch%20Sensor/5.%20LED%20nyala%20running%20saat%20sensor%20disentuh/touch_5.ino"> disini </a> atau dibawah ini
![LED nyala running saat sensor disentuh](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/83c476ae-a76f-447c-9ecf-2c20fee24fd4)

## 4. Kesimpulan

Program pada percobaan ini mengontrol beberapa LED menggunakan beberapa push button. Jika tombol pertama ditekan, LED pertama menyala atau mati. Tombol kedua membuat LED kedua berkedip dengan interval setengah detik. Saat tombol ketiga mengatur LED ketiga, keempat, dan kelima LED untuk berkedip secara bergantian dari kiri ke kanan. Program ini memberikan gambaran terhadap beberapa input tombol yang berbeda, dengan hasil ditampilkan di serial monitor.
