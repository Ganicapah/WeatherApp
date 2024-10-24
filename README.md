## Kelompok 11

1. Gani Samanta Capah - 1122091000065
2. Amir winanda - 11220910000052
3. Ahmad Rafiadly Arliansyah - 1120910000054

Project Link: [https://github.com/GaniCapah/WeatherApp](https://github.com/Ganicapah/WeatherApp)



# Weather App

Weather App adalah aplikasi Android sederhana yang menampilkan informasi cuaca untuk kota yang dipilih menggunakan OpenWeatherMap API. Aplikasi ini dibangun menggunakan Kotlin dan menampilkan berbagai informasi cuaca seperti suhu, kelembaban, tekanan udara, dan lainnya.


# User Interface
1. 
<img width="200" alt="Screenshot 2024-10-24 at 13 36 41" src="https://github.com/user-attachments/assets/e1afa5f4-1f04-4d2e-a025-5c5b1b310e09">



2. 
<img width="200" alt="Screenshot 2024-10-24 at 13 37 03" src="https://github.com/user-attachments/assets/cb8d72f3-c076-4230-8797-b7e3ee866dba">




## Fitur

- Menampilkan informasi cuaca real-time
- Pencarian kota
- Menampilkan berbagai informasi cuaca:
  - Suhu saat ini
  - Suhu minimum dan maksimum
  - Kelembaban
  - Tekanan udara
  - Kecepatan angin
  - Waktu matahari terbit dan terbenam
  - Deskripsi cuaca
- Auto-update informasi cuaca
- Tampilan loading saat mengambil data
- Penanganan error

## Persyaratan

- Android Studio
- Kotlin
- Minimum SDK: 30
- OpenWeatherMap API Key

## Instalasi

1. Clone repository ini
```bash
git clone https://github.com/Ganicapah/WeatherApp.git
```

2. Buka project di Android Studio

3. Dapatkan API Key dari [OpenWeatherMap](https://openweathermap.org/api)

4. Tambahkan API Key Anda di `MainActivity.kt`:
```kotlin
val API: String = "YOUR_API_KEY_HERE"
```

5. Build dan jalankan aplikasi

## Penggunaan

1. Saat pertama kali dibuka, aplikasi akan menampilkan cuaca untuk kota default (Jakarta)
2. Gunakan search bar di bagian atas untuk mencari kota lain
3. Masukkan nama kota dan tekan enter
4. Aplikasi akan menampilkan informasi cuaca untuk kota yang dipilih

## Struktur Kode

### MainActivity.kt
- `onCreate()`: Inisialisasi aplikasi dan setup SearchView
- `weatherTask`: Inner class yang menangani:
  - `onPreExecute()`: Menampilkan loading indicator
  - `doInBackground()`: Mengambil data dari API
  - `onPostExecute()`: Memproses response dan update UI

### Komponen Utama
- SearchView untuk input kota
- AsyncTask untuk network operations
- JSONObject untuk parsing data
- SimpleDateFormat untuk format waktu
- ProgressBar untuk loading indicator

## API Reference

Aplikasi ini menggunakan OpenWeatherMap API dengan endpoint:
```
https://api.openweathermap.org/data/2.5/weather
```

Parameter yang digunakan:
- `q`: Nama kota
- `units`: Metric (untuk Celsius)
- `appid`: API key

## Kontribusi

1. Fork repository
2. Buat branch fitur baru (`git checkout -b feature/AmazingFeature`)
3. Commit perubahan (`git commit -m 'Add some AmazingFeature'`)
4. Push ke branch (`git push origin feature/AmazingFeature`)
5. Buat Pull Request

## Unified Modeling Language

1. Activity Diagram
<img width="200" alt="ACTIVITY DIAGRAM" src="https://github.com/user-attachments/assets/fa4772d5-f7c5-4d78-bff3-aee7549e99b1">

2. State Diagram
<img width="200" alt="STATE DIAGRAM" src="https://github.com/user-attachments/assets/31b235d1-cc22-4c25-b931-7fb4fbd5562e">

3. Sequence Diagram
<img width="200" alt="SEQUENCE DIAGRAM" src="https://github.com/user-attachments/assets/18ff2059-732b-4fde-b485-246a8494982f">

4. Use Case Diagram
<img width="530" alt="USE CASE DIAGRAM" src="https://github.com/user-attachments/assets/0ac1713e-6aa9-4061-a578-f517b5328f42">


## Acknowledgments

- [OpenWeatherMap](https://openweathermap.org) untuk API cuaca
- [Android Developers](https://developer.android.com) untuk dokumentasi
- Semua kontributor yang telah membantu project ini
