# Jobsheet 2 - PROTOKOL KOMUNIKASI DAN SENSOR 

<p align="justify">ESP32 adalah nama dari mikrokontroler yang dirancang oleh perusahaan yang berbasis di Shanghai, China yakni Espressif Systems. ESP32 menawarkan solusi jaringan WiFi dan BLE. ESP32 menggunakan prosesor dual core yang berjalan di instruksi Xtensa LX16. Selain itu, ESP32 telah mendukung protokol komunikasi seperti I2C, UART dan SPI. Terdapat point penting dalam percobaan kali ini, yaitu :</p>

1. **UART (Universal Asynchronous Receiver Transmitter):** UART adalah protokol dalam pengiriman data serial antara device satu dengan lainnya. Dalam pengiriman data, clock antara pengirim dan penerima harus sama karena paket data dikirim tiap bit mengandalkan clock tersebut 
2. **SPI (Serial Peripheral Interface):** SPI adalah protokol komunikasi serial yang memungkinkan transfer data dengan kecepatan tinggi antara mikrokontroler dan perangkat lain. Protokol ini cocok untuk aplikasi yang membutuhkan transfer data dengan kecepatan tinggi, seperti pada layar LCD atau modul memori. SPI merupakan satu mode komunikasi serial synchrounous kecepatan tinggi yang dimiliki oleh Atmega 328. Komunikasi SPI membutuhkan 3 jalur yaitu MOSI, MISO, dan SCK.
3. **12C (Inter Integrated Circuit):** I2C adalah protokol komunikasi serial yang memungkinkan beberapa perangkat terhubung ke dalam satu bus. Protokol ini cocok untuk aplikasi yang membutuhkan komunikasi antara beberapa perangkat dengan menggunakan hanya dua kabel. Bus yang digunakan untuk komunikasi antara mikrokontroler dan device lainnya seperi sensor, dll.

Selamat mencoba dan semoga bermanfaat!

