# A. Setting SSID dan Password Wi-Fi ESP32 melalui Web Server

## 1. Alat dan Bahan
1) ESP32
2) Arduino IDE

## 2. Source Code

<img src="https://github.com/Aisyahnurul/AisyahN-system-embedded/assets/147674662/ea8c13bc-ceec-4e23-b6bd-782e1bcefb0c" width="700">

## 3. Flowchart
![jobsheet 4 A flowchart](https://github.com/Aisyahnurul/AisyahN-system-embedded/assets/147674662/26b1622e-6ddd-42bb-a2b7-6e63fca710a7)


## 4. Hasil dan Pembahasan
https://github.com/Aisyahnurul/AisyahN-system-embedded/assets/147674662/963a2b49-379b-498a-b700-5c8c3b3a7a36

<p align="justify">EPS32 akan menampilkan daftar SSID Wi-Fi yang tersedia pada serial monitor. Program mencoba terhubung ke jaringan WiFi yang telah disimpan dalam EEPROM (non-volatile memory). Jika koneksi WiFi gagal atau tombol fisik pada pin D15 (GPIO15) ditekan, program akan memulai konfigurasi sebagai titik akses (Access Point) untuk mengonfigurasi ulang WiFi. Output dari percobaan ini yaitu wifikampus succeessfully.
