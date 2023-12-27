# C. ESP-NOW | One-Way, One-to-Many Communication

## 1. Mengirim Pesan yang Sama ke Beberapa Board ESP32

### a. Rangkaian
Rangkaian pada percobaan ini adalah sebagai berikut
![rangkaian](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/f126fdf8-017f-4fb3-aa9f-f155d147785e)



### b. Source Code
Pada percobaan ini, kelompok kami sebagai Slave (receiver) <br>
Kode program dapat dilihat <a href="1.%20Mengirim%20Pesan%20yang%20Sama%20Ke%20Beberapa%20Board%20ESP32/4_ESP_collab/4_ESP_collab.ino">di sini</a>

### c. Hasil dan Pembahasan
Pada percobaan ini menggunakan 4 buah ESP32. Sebuah ESP akan menjadi Master (sender) dan 3 ESP lainnya menjadi Slave (receiver).
Master bertindak sebagai pengendali utama yang menginisiasi dan mengatur komunikasi, sementara 3 perangkat slave bertugas menerima instruksi atau data yang sama yang dikirimkan oleh master.
Pertama-tama, master memasukkan terlebih dahulu MAC Address dari masing-masing ESP yang menjadi slave. Kemudian master mengirimkan data yang sama kepada masing-masing slave.

##### Master

https://github.com/farhanhisyam/sistemEmbedded/assets/94108385/ab83cdf8-1cf1-4987-850b-ccb24efa5dce

##### Slave

https://github.com/farhanhisyam/sistemEmbedded/assets/94108385/ddfe26be-7e7c-47a4-9a9f-d921bbe5b6a3


##### Salah satu board slave dimatikan
Jika salah satu board slave dimatikan=, maka komunikasi antara master dan slave tersebut akan terputus. Master tidak akan dapat mengirimkan instruksi atau data ke perangkat slave yang dimatikan tersebut, dan slave yang dimatikan juga tidak akan dapat merespons atau menerima data.

https://github.com/farhanhisyam/sistemEmbedded/assets/94108385/5a5ce77b-8112-4b29-ae5a-ac7749779e1e


## 2. Mengirim Pesan yang Berbeda ke Beberapa Board ESP32

### a. Rangkaian
Rangkaian pada percobaan ini adalah sebagai berikut
![rangkaian](https://github.com/sabrinavirry/Sistem-Embedded/assets/151721571/68c9666a-8057-4de9-a293-d03f51338aaa)



### b. Source Code
Pada percobaan ini, kelompok kami sebagai Master (sender) <br>
Kode program dapat dilihat <a href="2.%20Mengirim%20Pesan%20yang%20Berbeda%20Ke%20Beberapa%20Board%20ESP32/4_ESP_collab_beda_pesan/4_ESP_collab_beda_pesan.ino">di sini</a>

### c. Hasil dan Pembahasan
Pada percobaan ini konfigurasinya masih sama dengan sebelumnya, yaitu 1 ESP bertindak sebagai Master dan 3 ESP bertindak sebagai Slave. Yang membedakan adalah data
yang dikirimkan kepada masing-masing Slave berbeda. Slave 1 akan mendapatkan data yang berisi variabel dengan tipe data integer, slave 2 mendapatkan data variabel dengan tipe data float, 
dan slave 3 mendapatkan data variabel dengan tipe data string.


##### Master

https://github.com/farhanhisyam/sistemEmbedded/assets/94108385/dd169363-03e4-431c-867c-eb39e005783c

##### Slave 1

https://github.com/farhanhisyam/sistemEmbedded/assets/94108385/ae24f108-ac93-48d1-84f8-21e5d4afe44b

##### Slave 2

https://github.com/farhanhisyam/sistemEmbedded/assets/94108385/d9c1da13-dce7-4f1c-8ec9-c8ff383a34ea

##### Slave 3

https://github.com/farhanhisyam/sistemEmbedded/assets/94108385/6440d876-757b-48c9-9ec7-46926fa2eb4d


