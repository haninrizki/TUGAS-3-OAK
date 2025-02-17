# TUGAS-3-OAK 
#09011182429010_M.Hanindita
![image](https://github.com/user-attachments/assets/7125c4fc-1f78-46e9-af20-3ffa06300fa0)
ESP8266 adalah microcontroller dengan WiFi bawaan, digunakan untuk IoT, smart home, dan automasi. Sebagai control unit, ESP8266 berfungsi untuk membaca sensor, memproses data, dan mengontrol perangkat elektronik melalui GPIO, PWM, ADC, I2C, SPI, UART, dan WiFi.

1. Arsitektur Control Unit ESP8266
Sebagai control unit, ESP8266 mengontrol perangkat melalui beberapa antarmuka berikut:

1.1. GPIO (General Purpose Input Output)
Fungsi: Mengontrol perangkat digital seperti relay, LED, tombol.
Jumlah: 9 GPIO (pada ESP-12E/F, NodeMCU).
Contoh:
✅ Menyalakan LED atau relay dengan GPIO output.
✅ Membaca tombol atau sensor gerak (PIR) dengan GPIO input.
1.2. PWM (Pulse Width Modulation)
Fungsi: Mengontrol kecepatan motor, kecerahan LED, atau sudut servo.
Contoh:
✅ Mengontrol kecepatan kipas DC berdasarkan suhu.
✅ Mengontrol servo untuk robotik.
1.3. ADC (Analog to Digital Converter)
Fungsi: Membaca sensor analog seperti LDR, potensiometer, sensor suhu LM35.
Jumlah: 1 pin ADC (10-bit resolusi, maks 1V input).
Contoh:
✅ Membaca sensor suhu LM35 untuk monitoring suhu ruangan.
1.4. I2C (Inter-Integrated Circuit)
Fungsi: Berkomunikasi dengan sensor atau modul I2C.
Contoh:
✅ Menampilkan data di OLED Display SSD1306.
✅ Membaca sensor suhu & kelembaban DHT22.
1.5. SPI (Serial Peripheral Interface)
Fungsi: Berkomunikasi dengan perangkat berkecepatan tinggi seperti kartu SD atau layar TFT.
Contoh:
✅ Menghubungkan modul RFID MFRC522.
✅ Menyimpan data pada microSD.
1.6. UART (Universal Asynchronous Receiver-Transmitter)
Fungsi: Berkomunikasi dengan modul eksternal seperti GPS atau sensor serial.
Contoh:
✅ Menghubungkan modul GPS NEO-6M untuk tracking.
✅ Berkomunikasi dengan Arduino atau Raspberry Pi.
1.7. WiFi (802.11 b/g/n)
Fungsi: Menghubungkan ESP8266 ke Internet atau perangkat lain.
Contoh:
✅ Mengontrol lampu dari aplikasi mobile via WiFi.
✅ Mengirim data sensor ke cloud (MQTT, Firebase, ThingSpeak).

![image](https://github.com/user-attachments/assets/b3ea127f-ffce-4018-be92-ff58b5423ac4)
Raspberry Pi 5 adalah single-board computer (SBC) terbaru dari Raspberry Pi Foundation yang memiliki peningkatan performa signifikan dibanding pendahulunya. Sebagai control unit, Raspberry Pi 5 mampu mengontrol berbagai perangkat melalui GPIO, I2C, SPI, UART, PWM, dan PCIe, serta mendukung WiFi dan Bluetooth untuk komunikasi jaringan.

Fitur Control Unit pada Raspberry Pi 5
Raspberry Pi 5 bisa berfungsi sebagai control unit dalam berbagai aplikasi, mulai dari otomasi industri, IoT, robotika, hingga AI/ML. Berikut beberapa fitur utama yang digunakan untuk kontrol perangkat:

2.1. GPIO (General Purpose Input/Output)
Jumlah: 40 pin GPIO (3.3V logic level)
Fungsi: Mengontrol perangkat elektronik seperti relay, motor, LED, sensor.
Contoh Penggunaan: ✅ Mengontrol lampu pintar dengan relay.
✅ Membaca status tombol atau sensor gerak (PIR).
2.2. PWM (Pulse Width Modulation)
Fungsi: Mengontrol motor servo, LED dimming, dan aktuator lainnya.
Contoh Penggunaan: ✅ Mengontrol motor servo SG90 untuk proyek robot.
✅ Mengatur kecepatan kipas berdasarkan suhu CPU.
2.3. I2C (Inter-Integrated Circuit)
Jumlah: 4 bus I2C.
Fungsi: Berkomunikasi dengan sensor dan modul eksternal.
Contoh Penggunaan: ✅ Membaca data dari sensor suhu & kelembaban (BME280, DHT22).
✅ Menghubungkan LCD 16x2 I2C untuk menampilkan informasi.
2.4. SPI (Serial Peripheral Interface)
Jumlah: 6 bus SPI.
Fungsi: Berkomunikasi dengan sensor kecepatan tinggi atau modul memori.
Contoh Penggunaan: ✅ Menghubungkan modul RFID MFRC522 untuk akses kontrol.
✅ Menggunakan modul LoRa SX1278 untuk komunikasi jarak jauh.
2.5. UART (Universal Asynchronous Receiver-Transmitter)
Jumlah: 6 port UART.
Fungsi: Komunikasi serial dengan mikrokontroler atau perangkat lain.
Contoh Penggunaan: ✅ Menghubungkan Arduino ke Raspberry Pi 5.
✅ Berkomunikasi dengan modul GSM/GPS (SIM800L, NEO-6M).
2.6. PCIe 2.0 (Peripheral Component Interconnect Express)
Fungsi: Memungkinkan penggunaan SSD NVMe, AI accelerator, atau kartu jaringan tambahan.
Contoh Penggunaan: ✅ Menjalankan AI/ML dengan Coral Edge TPU atau Hailo AI Accelerator.
✅ Menyimpan data lebih cepat dengan SSD NVMe PCIe.
2.7. WiFi 5 & Gigabit Ethernet
Fungsi: Memungkinkan kontrol perangkat melalui jaringan internet.
Contoh Penggunaan: ✅ Mengontrol smart home dari jarak jauh dengan Home Assistant.
✅ Membuat server IoT untuk data logging dan kontrol jarak jauh.
