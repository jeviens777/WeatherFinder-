# 🌤️ WeatherFinder

WeatherFinder adalah aplikasi React Native yang memungkinkan pengguna mencari informasi cuaca secara real-time berdasarkan nama kota menggunakan API gratis dari Open-Meteo.

Aplikasi ini dibuat menggunakan React Native dan menerapkan konsep penting seperti useState, useEffect, debounce, fetch API, cleanup function, AbortController, dan conditional rendering.

---

## 📱 Fitur Aplikasi

### ✅ Level 1 (Fitur Wajib)

- TextInput (Controlled Component)
- Debounce 500ms menggunakan setTimeout dan clearTimeout
- useEffect dengan dependency array `[searchInput]`
- Fetch API Open-Meteo (2 langkah):
  - Geocoding (Nama Kota → Koordinat)
  - Forecast (Koordinat → Data Cuaca)
- Loading State dengan ActivityIndicator
- Error State
- Empty State
- Success State
- AbortController untuk membatalkan request lama
- Mapping Weather Code (WMO) ke label dan emoji
- Menampilkan:
  - Nama Kota
  - Negara
  - Suhu Saat Ini
  - Kondisi Cuaca

---

### 🟡 Level 2 (Fitur Pengembangan yang Dipilih)

#### ✅ Arah & Kecepatan Angin

Menampilkan:
- Kecepatan angin (km/h)
- Arah mata angin (U, TL, T, TG, S, BD, B, BL)

#### ✅ Suhu Minimum & Maksimum Harian

Menampilkan:
- Suhu minimum harian
- Suhu maksimum harian

#### ✅ Riwayat Pencarian

- Menyimpan 5 kota terakhir yang dicari
- Dapat ditekan kembali untuk mencari ulang

#### ✅ Background Dinamis

Warna kartu cuaca berubah sesuai kondisi:

| Kondisi | Warna |
|----------|---------|
| Cerah ☀️ | Kuning |
| Berawan ⛅ | Biru |
| Mendung ☁️ | Abu-abu |
| Hujan 🌧️ | Biru Gelap |
| Badai ⛈️ | Biru Sangat Gelap |

---

## 🛠️ Teknologi yang Digunakan

- React Native
- Expo
- JavaScript
- Open-Meteo API

---

## 🌍 API yang Digunakan

### Geocoding API

Mengubah nama kota menjadi koordinat.

```url
https://geocoding-api.open-meteo.com/v1/search
```

### Forecast API

Mengambil data cuaca berdasarkan koordinat.

```url
https://api.open-meteo.com/v1/forecast
```

API ini gratis dan tidak memerlukan API Key.

---

## 🚀 Cara Menjalankan Project

### 1. Clone Repository

```bash
git clone https://github.com/USERNAME/weather-finder.git
```

### 2. Masuk ke Folder Project

```bash
cd weather-finder
```

### 3. Install Dependencies

```bash
npm install
```

atau

```bash
yarn install
```

---

### 4. Jalankan Expo

```bash
npx expo start
```

---

### 5. Jalankan di Device

Pilih salah satu:

- Android Emulator
- iOS Simulator
- Expo Go (Android/iPhone)

Scan QR Code yang muncul setelah Expo berjalan.

---

## 📂 Struktur Project

```text
WeatherFinder
│
├── assets/
├── App.js
├── package.json
├── package-lock.json
└── README.md
```

---

## 👨‍💻 Konsep React Native yang Digunakan

- Functional Component
- useState
- useEffect
- Controlled Component
- Conditional Rendering
- Fetch API
- Async Request Handling
- Debounce
- Cleanup Function
- AbortController
- Dynamic Styling

---

## 📸 Tampilan Aplikasi
![Kosong Screen](assets/kosong.jpeg)





## 👤 Author

Nama: [Jeviens Paradisa Finie Adena]

Mata Kuliah: React Native

Project: WeatherFinder
