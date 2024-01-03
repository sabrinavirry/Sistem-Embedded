# C. ESP-NOW | One-Way, One-to-Many Communication

## 1. Mengirim Pesan yang Sama ke Beberapa Board ESP32

### a. Rangkaian
Rangkaian pada percobaan ini adalah sebagai berikut
![rangkaian](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/f126fdf8-017f-4fb3-aa9f-f155d147785e)



### b. Source Code
Pada percobaan ini, kelompok kami sebagai Slave (receiver) <br>
Program dapat dilihat dibawah ini atau dapat klik <a href="https://github.com/sabrinavirry/Sistem-Embedded/blob/master/jobsheet%202.1/c.%20One-Way%2C%20One-to-Many%20Communication/1.%20Mengirim%20Pesan%20yang%20Sama%20Ke%20Beberapa%20Board%20ESP32/receiver.ino">di sini</a>
![receiver](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/cb13ef31-4bb2-4a3e-a646-32e81c06c290)


### c. Hasil dan Pembahasan
Pada percobaan ini menggunakan 4 buah ESP32. Sebuah ESP akan menjadi Master (sender) dan 3 ESP lainnya menjadi Slave (receiver).
Master bertindak sebagai pengendali utama yang menginisiasi dan mengatur komunikasi, sementara 3 perangkat slave bertugas menerima instruksi atau data yang sama yang dikirimkan oleh master.
Pertama-tama, master memasukkan terlebih dahulu MAC Address dari masing-masing ESP yang menjadi slave. Kemudian master mengirimkan data yang sama kepada masing-masing slave.

![J2 1 -C-1-1](https://github.com/brianrahma/system-embedded/assets/82065700/48437206-8f7a-4bdc-aa1c-5e62e8337466)

<p align="justify">Pada percobaan ini  menggunakan empat modul ESP32, di mana satu modul berperan sebagai Master/sender dan tiga modul lainnya sebagai receiver. Langkah awal memerlukan MAC Address dari tiap ESP32 yang akan menjadi receivernya, diikuti dengan memasukkan MAC address receiver pada program Master untuk mengirimkan data seragam ke setiap modul receiver. Program tersebut diunggah ke masing-masing modul, dan kemudian dilakukan pemantauan melalui Serial Monitor di Arduino IDE.

**Apabila salah satu board Receiver dimatikan**

![J2 1 -C-1-1](https://github.com/brianrahma/system-embedded/assets/82065700/6a07e44b-3b04-45fe-984e-db32e085ddab)

<p align="justify">Yang terjadi adalah komunikasi antara sender dan receiver akan terputus, artinya data yang dikirim sender tidak akan diterima oleh receiver, dan pada sender tercetak "Delivery Fail"


## 2. Mengirim Pesan yang Berbeda ke Beberapa Board ESP32

### a. Rangkaian
Rangkaian pada percobaan ini adalah sebagai berikut
![rangkaian](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/68c9666a-8057-4de9-a293-d03f51338aaa)



### b. Source Code
Pada percobaan ini, kelompok kami sebagai Master (sender) <br>
Program dapat dilihat dibawah ini atau dapat klik <a href="https://github.com/sabrinavirry/Sistem-Embedded/blob/master/jobsheet%202.1/c.%20One-Way,%20One-to-Many%20Communication/2.%20Mengirim%20Pesan%20yang%20Berbeda%20Ke%20Beberapa%20Board%20ESP32/_receive_mac_Mengirim_Pesan_yang_Berbeda_Ke_Beberapa_Board_ESP3.ino">di sini</a>
![receive mac](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/0bf930f6-3f86-48a0-8ede-9f60d20fca17)


### c. Hasil dan Pembahasan

![J2 1 -C-1-2](https://github.com/brianrahma/system-embedded/assets/82065700/a764446b-a2b5-48d5-9c07-44a05253ca96)

<p align="justify">Pada percobaan ini masih sama dengan sebelumnya, yaitu menggunakan 1 ESP yang bertindak sebagai Master/sender dan 3 ESP bertindak sebagai receiver. Perbedaannya terdapat pada data yang dikirimkan ke masing-masing receiver tidak sama. Receiver 1 akan mendapatkan data yang berisi variabel dengan tipe data integer, receiver 2 mendapatkan data variabel dengan tipe data float, dan receiver 3 mendapatkan data variabel dengan tipe data string.

