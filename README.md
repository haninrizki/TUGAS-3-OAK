# TUGAS-3-OAK 
# 09011182429010_M.Hanindita
![image](https://github.com/user-attachments/assets/7125c4fc-1f78-46e9-af20-3ffa06300fa0)

ESP8266 adalah microcontroller dengan WiFi bawaan, digunakan untuk IoT, smart home, dan automasi. Sebagai control unit, ESP8266 berfungsi untuk membaca sensor, memproses data, dan mengontrol perangkat elektronik melalui GPIO, PWM, ADC, I2C, SPI, UART, dan WiFi.

# 1. Arsitektur Control Unit ESP8266
Sebagai control unit, ESP8266 mengontrol perangkat melalui beberapa antarmuka berikut:
# 1.1. GPIO (General Purpose Input Output)
Fungsi: Mengontrol perangkat digital seperti relay, LED, tombol.
Jumlah: 9 GPIO (pada ESP-12E/F, NodeMCU).

Contoh:

=> Menyalakan LED atau relay dengan GPIO output.

=> Membaca tombol atau sensor gerak (PIR) dengan GPIO input.
# 1.2. PWM (Pulse Width Modulation)
Fungsi: Mengontrol kecepatan motor, kecerahan LED, atau sudut servo.

Contoh:

=> Mengontrol kecepatan kipas DC berdasarkan suhu.

=> Mengontrol servo untuk robotik.
# 1.3. ADC (Analog to Digital Converter)
Fungsi: Membaca sensor analog seperti LDR, potensiometer, sensor suhu LM35.
Jumlah: 1 pin ADC (10-bit resolusi, maks 1V input).

Contoh:

=>  Membaca sensor suhu LM35 untuk monitoring suhu ruangan.

# 1.4. I2C (Inter-Integrated Circuit)
Fungsi: Berkomunikasi dengan sensor atau modul I2C.

Contoh:

=>  Menampilkan data di OLED Display SSD1306.

=> Membaca sensor suhu & kelembaban DHT22.
# 1.5. SPI (Serial Peripheral Interface)
Fungsi: Berkomunikasi dengan perangkat berkecepatan tinggi seperti kartu SD atau layar TFT.

Contoh:

=> Menghubungkan modul RFID MFRC522.

=> Menyimpan data pada microSD.
# 1.6. UART (Universal Asynchronous Receiver-Transmitter)
Fungsi: Berkomunikasi dengan modul eksternal seperti GPS atau sensor serial.

Contoh:

=> Menghubungkan modul GPS NEO-6M untuk tracking.

=> Berkomunikasi dengan Arduino atau Raspberry Pi.
# 1.7. WiFi (802.11 b/g/n)
Fungsi: Menghubungkan ESP8266 ke Internet atau perangkat lain.

Contoh:

=> Mengontrol lampu dari aplikasi mobile via WiFi.

=> Mengirim data sensor ke cloud (MQTT, Firebase, ThingSpeak).

## Cara kerja ESP8266
# 1.Inisialisasi
ESP8266 dinyalakan dan mulai menjalankan firmware yang ada di dalamnya.
Modul dapat dikonfigurasi sebagai Access Point (AP) atau Station (STA).

# 2.Koneksi ke WiFi
Jika dalam mode STA, ESP8266 akan mencari jaringan WiFi yang tersedia dan terhubung ke SSID yang diatur.
Jika dalam mode AP, ESP8266 membuat jaringan sendiri agar perangkat lain dapat terhubung.
Komunikasi Data

# 3.Menggunakan protokol TCP/IP untuk mengirim dan menerima data dari server atau perangkat lain.
Dapat mengakses layanan berbasis HTTP (seperti API atau website).
Bisa berfungsi sebagai Web Server untuk menampilkan halaman atau menerima input dari pengguna.

# 4.Interaksi dengan Perangkat Lain
ESP8266 dapat membaca sensor melalui pin GPIO dan mengirim data ke server.
Bisa mengontrol aktuator seperti relay atau LED berdasarkan instruksi yang diterima melalui internet.

# Mode Operasi ESP8266
Mode Station (STA): Terhubung ke router WiFi dan bertindak sebagai klien.
Mode Access Point (AP): Membuat jaringan WiFi sendiri untuk perangkat lain.
Mode Dual (AP + STA): Bisa terhubung ke WiFi dan membuat jaringan sendiri secara bersamaan.

 # Pemrograman ESP8266
ESP8266 dapat diprogram menggunakan:
Arduino IDE: Menggunakan library seperti ESP8266WiFi.h
Lua (NodeMCU): Menggunakan script Lua dengan firmware NodeMCU.
MicroPython: Menggunakan bahasa Python untuk pengendalian lebih fleksibel.

# Kesimpulan
ESP8266 adalah modul WiFi yang murah dan fleksibel untuk proyek IoT. Dengan kemampuan komunikasi jaringan yang baik dan kompatibilitas dengan berbagai platform pemrograman, ESP8266 banyak digunakan dalam smart home, monitoring sensor, dan kontrol perangkat jarak jauh.

