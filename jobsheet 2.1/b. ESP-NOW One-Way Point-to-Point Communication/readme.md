# B. ESP-NOW | One-Way Point-to-Point Communication

## 1. Basic

### a. Rangkaian
Rangkaian pada percobaan ini adalah sebagai berikut

![image](https://github.com/farhanhisyam/sistemEmbedded/assets/94108385/d66c1441-4e2b-402e-9b6a-a2fff986e1ef)

### b. Source Code
Pada percobaan ini, kelompok kami sebagai receiver <br>
Kode program dapat dilihat <a href="ESP-NOW_One-Way_Point-to-Point_Communication/ESP-NOW_One-Way_Point-to-Point_Communication.ino">di sini</a>

### c. Hasil dan Pembahasan
Program dibagi menjadi 2, yaitu sender dan receiver<br>
Penjelasan program sender adalah sebagai berikut

1. Include Library dan Header
```c
#include <esp_now.h>
#include <WiFi.h>
```
>Program ini menggunakan dua library, yaitu `esp_now` untuk ESP-NOW dan `WiFi` untuk mengonfigurasi mode WiFi.
<br>

2. Inisialisasi Broadcast Address
```c
uint8_t broadcastAddress[] = {0xFF, 0xFF, 0xFF, 0xFF, 0xFF, 0xFF};
```
>Menginisialisasi alamat broadcast yang digunakan untuk mengirim data ke semua perangkat di jaringan.
<br>

  3. Deklarasi Struktur Pesan
```c
typedef struct struct_message {
    char a[32];
    int b;
    float c;
    bool d;
} struct_message;
```
>Mendefinisikan struktur pesan yang akan dikirim. Struktur ini memiliki empat elemen, yaitu array karakter, integer, float, dan boolean.
<br>

  4. Deklarasi Variabel dan Fungsi Callback
```c
struct_message myData;
esp_now_peer_info_t peerInfo;

void OnDataSent(const uint8_t *mac_addr, esp_now_send_status_t status) {
    Serial.print("\r\nStatus Paket Terakhir :\t");
    Serial.println(status == ESP_NOW_SEND_SUCCESS ? "Sukses Terkirim" : "Gagal Terkirim");
}
```
>Menyediakan variabel untuk menyimpan data yang akan dikirim dan struktur peer info untuk informasi penerima. Fungsi `OnDataSent` adalah callback yang dipanggil setelah data terkirim.
<br>

  5. Setup Function
```c
void setup() {
    Serial.begin(115200);
    WiFi.mode(WIFI_STA);

    if (esp_now_init() != ESP_OK) {
        Serial.println("Gagal menginisialisasi ESP-NOW");
        return;
    }

    esp_now_register_send_cb(OnDataSent);

    memcpy(peerInfo.peer_addr, broadcastAddress, 6);
    peerInfo.channel = 0;
    peerInfo.encrypt = false;

    if (esp_now_add_peer(&peerInfo) != ESP_OK){
        Serial.println("Gagal menambahkan peer");
        return;
    }
}
```
 > - Menginisialisasi Serial Monitor dan mode WiFi sebagai station.
 > - Menginisialisasi ESP-NOW dan mendaftarkan callback untuk meng-handle status pengiriman.
 > - Mendaftarkan alamat peer yang akan menerima data.
<br>

  6. Loop Function
```c
void loop() {
    strcpy(myData.a, "INI ADALAH CHAR");
    myData.b = random(1,20);
    myData.c = 1.2;
    myData.d = false;

    esp_err_t result = esp_now_send(broadcastAddress, (uint8_t *) &myData, sizeof(myData));

    if (result == ESP_OK) {
        Serial.println("Data berhasil terkirim");
    }
    else {
        Serial.println("Gagal mengirim data");
    }

    delay(2000);
}
```
 > - Mengisi data dalam struktur pesan.
 > - Mengirim data menggunakan `esp_now_send`.
 > - Menampilkan status pengiriman data melalui Serial Monitor.
 > - Menunggu selama 2 detik sebelum mengulang proses pengiriman.
Dengan demikian, program ini secara berulang mengirim data menggunakan protokol ESP-NOW ke perangkat penerima yang telah ditentukan.
<br>

Sedangkan penjelasan program receiver adalah sebagai berikut
  1. Include Library dan Header
```c
#include <esp_now.h>
#include <WiFi.h>
```
>Seperti pada program sender, library yang digunakan adalah `esp_now` untuk ESP-NOW dan `WiFi` untuk mengonfigurasi mode WiFi.
<br>
  
  2. Deklarasi Struktur Pesan
```c
typedef struct struct_message {
    char a[32];
    int b;
    float c;
    bool d;
} struct_message;
```
>Mendefinisikan struktur pesan yang harus sama dengan struktur pesan pada program sender untuk memastikan konsistensi data yang dikirim dan diterima.
<br>
  
  3. Deklarasi Variabel dan Fungsi Callback Penerima
```c
struct_message myData;

void OnDataRecv(const uint8_t * mac, const uint8_t *incomingData, int len) {
    // Mengkopi data yang diterima ke dalam struktur myData
    memcpy(&myData, incomingData, sizeof(myData));

    // Menampilkan data yang diterima melalui Serial Monitor
    Serial.print("Bytes received: ");
    Serial.println(len);
    Serial.print("Char: ");
    Serial.println(myData.a);
    Serial.print("Int: ");
    Serial.println(myData.b);
    Serial.print("Float: ");
    Serial.println(myData.c);
    Serial.print("Bool: ");
    Serial.println(myData.d);
    Serial.println();
}
```
>`OnDataRecv`: Callback yang dieksekusi ketika ada data yang diterima. Menggunakan `memcpy` untuk menyalin data yang diterima ke dalam struktur `myData`. Kemudian, menampilkan informasi mengenai data yang diterima melalui Serial Monitor.
<br>
  
  4. Setup Function
```c
void setup() {
    // Initialize Serial Monitor
    Serial.begin(115200);
    
    // Set ESP32 sebagai station
    WiFi.mode(WIFI_STA);

    // Inisialisasi ESP-NOW dan mendaftarkan callback untuk proses penerimaan data
    if (esp_now_init() != ESP_OK) {
        Serial.println("Error initializing ESP-NOW");
        return;
    }
    esp_now_register_recv_cb(OnDataRecv);
}
```
 > - Menginisialisasi Serial Monitor dan mode WiFi sebagai station.
 > - Inisialisasi ESP-NOW dan mendaftarkan callback `OnDataRecv` untuk menangani proses penerimaan data.
<br>
  
  5. Loop Function
```c
void loop() {
    // Loop kosong, karena penerima hanya menangani data yang diterima secara asinkron.
}
```
>Loop utama tidak melakukan apa-apa karena penerima hanya menangani data yang diterima secara asinkron melalui callback.
Program ini, ketika dijalankan, akan terus mendengarkan dan menampilkan informasi mengenai data yang diterima melalui protokol ESP-NOW. Program sender yang sesuai akan mengirimkan data ke ESP32 yang berperan sebagai receiver, dan callback OnDataRecv akan dieksekusi untuk menangani data yang diterima.
<br>

Sehingga output yang dihasilkan adalah pada serial monitor sender akan menghasilkan output berupa “Data berhasil dikirim” sedangkan pada serial monitor receiver output yang dihasilkan berupa “INI ADALAH CHAR”

##### Sender

![hasil-2-kirim](https://github.com/farhanhisyam/sistemEmbedded/assets/94108385/df255ae8-f4ba-4825-b912-745a7c448b16)

##### Receiver

![hasil-2-terima](https://github.com/farhanhisyam/sistemEmbedded/assets/94108385/27ebaf82-6649-47d1-aa73-b34c9704a9be)

Untuk mengirimkan data dummy dengan ukuran yang terbaca oleh receiver $\pm$ 250 byte, yang harus dilakukan adalah dengan mengubah nilai `char a[]` menjadi 236
```c
typedef struct struct_message {
 char a[236];
 int b;
 float c;
 bool d;
}
```
Hasilnya adalah sebagai berikut

##### Sender
![hasil-2-248byte-kirim](https://github.com/farhanhisyam/sistemEmbedded/assets/94108385/3154b101-b039-4eaa-a9ae-57a1d33ec208)

##### Receiver
![hasil-2-248byte-terima](https://github.com/farhanhisyam/sistemEmbedded/assets/94108385/c6fac252-8990-4f3e-8208-cff084d8a9d0)

## 2. Tugas

### a. Rangkaian
Rangkaian pada percobaan ini adalah sebagai berikut

![image](https://github.com/farhanhisyam/sistemEmbedded/assets/94108385/d66c1441-4e2b-402e-9b6a-a2fff986e1ef)

### b. Source Code
Pada percobaan ini, kelompok kami sebagai receiver <br>
Kode program dapat dilihat <a href="ESP-NOW_One-Way_Point-to-Point_Communication/ESP-NOW_One-Way_Point-to-Point_Communication.ino">di sini</a>

### c. Hasil dan Pembahasan
Pada percobaan ini, pengiriman Point-to-Point dilakukan dalam beberapa kondisi. Pertama, ada 3 kondisi jarak transmisi yaitu 1 meter, 2 meter, dan 3 meter. Kemudian, pada masing-masing jarak diberikan 3 kondisi ketinggian yaitu ground, 30cm, dan 1 meter diatas permukaan tanah. Hasil pemantauan jumlah data yang berhasil terkirim dan diterima adalah sebagai berikut

##### Hasil Kirim

https://github.com/farhanhisyam/sistemEmbedded/assets/94108385/7c8f8ee8-2fbf-4037-9a62-cff7d6fa6b30


##### Hasil Terima

https://github.com/farhanhisyam/sistemEmbedded/assets/94108385/11227fda-bc07-43f6-a893-9f8620bbc431


##### Hasil Tabel

![hasil-tabel](https://github.com/farhanhisyam/sistemEmbedded/assets/94108385/2c8a7c40-5940-488a-936d-28a75955d725)
>*Note: Dokumentasi percobaan dapat dilihat pada folder "dokumentasi"*

Dari hasil tabel diatas dapat dilihat bahwa pengiriman berjalan dengan baik dalam segala kondisi. Persentase packet loss adalah 0% dengan keberhasilan pengiriman 100%. 

