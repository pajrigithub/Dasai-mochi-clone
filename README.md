# OLED Animation with ESP32

Animasi gambar (seperti GIF) ke layar OLED menggunakan ESP32 dan library `Adafruit_SSD1306`. Gambar animasi dikonversi menjadi file header (`.h`) berisi array bitmap, lalu ditampilkan frame per frame di OLED.

## 📦 Fitur

- Menampilkan animasi bitmap (seperti GIF) di OLED 128x64
- File `.h` otomatis hasil konversi dari script Python/tool
- Mudah diubah jadi template untuk berbagai animasi

## 🚀 Langkah-langkah Penggunaan

1. **Ekstrak Folder `dist`**  
   Ekstrak terlebih dahulu folder `dist` yang berisi tool converter bernama `gif2oled`.

2. **Jalankan `gif2oled`**  
   Buka program `gif2oled.exe` yang terdapat di dalam folder hasil ekstrak.

3. **Masukkan Path File GIF**  
   Saat diminta, masukkan path lengkap ke file GIF yang ingin kamu konversi (pake tanda "").  
   Contoh:  "C:\Users\MyBook Hype\Downloads\RobotFace(DasaiMociClone)\Animasi & Converter GIF\angry.gif"

4. **Setel Nilai Threshold (Default: 100)**  
Threshold digunakan untuk mengatur tingkat noise dari GIF.  
Semakin tinggi nilainya, semakin bersih hasil konversi.  
Jika ragu, gunakan nilai default `100`.

5. **Lihat Hasil di Folder `dist`**  
Setelah proses selesai, hasil konversi akan otomatis tersimpan di dalam folder `dist`.

6. **Masukkan Hasil ke Kode Arduino example_dasai_clone**  
Gunakan file hasil konversi `.h` ke dalam kode Arduino yang telah disediakan.  
File tersebut berisi array bitmap yang siap ditampilkan pada OLED.

📌 **Catatan:**
- Pastikan resolusi GIF sesuai dengan ukuran OLED (biasanya 128x64).
- Gunakan GIF dengan background kontras tinggi untuk hasil terbaik.


