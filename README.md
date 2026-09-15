# 📦 RentIT - Peer-to-Peer Universal Rental Marketplace

<p align="center">
  <img src="https://img.shields.io/badge/Flutter-3.x-02569B?logo=flutter&logoColor=white" alt="Flutter Version" />
  <img src="https://img.shields.io/badge/Dart-3.x-0175C2?logo=dart&logoColor=white" alt="Dart Version" />
  <img src="https://img.shields.io/badge/Platform-iOS%20%7C%20Android-green" alt="Platforms" />
  <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License" />
</p>

<p align="center">
  <b>Sewa apa saja, kapan saja. Pinjam yang kamu butuhkan, hasilkan uang dari barangmu.</b><br>
  <i>(A cross-platform community rental marketplace mobile application built with Flutter).</i>
</p>

---

## 📖 Ringkasan Proyek (Overview)

**RentIT** adalah aplikasi mobile cross-platform berbasis **Flutter** yang menghubungkan pemilik barang dengan penyewa di sekitar area mereka secara aman, cepat, dan mudah.

Alih-alih membeli barang mahal yang hanya digunakan sesekali (seperti kamera, drone, tenda camping, perkakas listrik, proyektor, hingga jas/kostum pesta), pengguna dapat menyewanya dengan harga terjangkau. Di sisi lain, pemilik barang dapat menghasilkan pendapatan pasif dari barang-barang yang menganggur di rumah.

---

## ✨ Fitur Utama (Key Features)

- 📍 **Peta & Eksplorasi Sekitar (Nearby Map & Search)**: Temukan barang sewaan di radius terdekat dari lokasi pengguna secara real-time.
- 📅 **Kalender Sewa & Booking Dinamis**: Pilih durasi sewa fleksibel (harian, mingguan, bulanan) dengan pengecekan ketersediaan instan.
- 💬 **In-App Real-time Chat**: Komunikasi langsung antara penyewa dan pemilik barang untuk konsultasi spesifikasi serta janji temu serah-terima.
- 💳 **Pembayaran Aman & Penahanan Deposit**: Pembayaran in-app dengan fitur *deposit hold* untuk perlindungan barang dan keamanan transaksi.
- 📸 **Inspeksi Serah-Terima (Check-In & Check-Out)**: Dokumentasi foto kondisi fisik barang sebelum dan sesudah masa sewa untuk transparansi.
- 🛡️ **Verifikasi Identitas & Reputasi Komunitas**: Verifikasi identitas (KYC/ID) serta sistem ulasan dan rating dua arah (*two-way review*).

---

## 🛠️ Tech Stack & Ekosistem

* **Framework:** [Flutter](https://flutter.dev/) (Dart)
* **State Management:** Riverpod (`flutter_riverpod`) / BLoC
* **Navigasi & Routing:** `go_router`
* **Maps & Geolocation:** `google_maps_flutter`, `geolocator`
* **Backend & Database:** [Supabase](https://supabase.com/) / Firebase (Auth, PostgreSQL, Realtime, Storage)
* **Payment Gateway:** Stripe (`flutter_stripe`) / Midtrans / Xendit
* **Image Picker & Cache:** `image_picker`, `cached_network_image`

---

## 📂 Struktur Arsitektur Folder (Feature-First)

```text
lib/
├── core/                  # Komponen global, tema, konstanta, network client
│   ├── constants/         # App constants, warna, aset
│   ├── network/           # API Client / Supabase Client
│   ├── theme/             # Light & Dark Theme Data
│   └── utils/             # Helper format tanggal, mata uang, validasi
├── features/              # Modul berbasis fitur
│   ├── auth/              # Login, Register, KYC Verifikasi
│   ├── browse/            # Beranda, Filter Kategori, Peta Sekitar
│   ├── item_details/      # Halaman Detail Barang, Galeri Foto
│   ├── booking/           # Kalender Sewa, Checkout, Pembayaran & Deposit
│   ├── listing/           # Form Tambah Barang & Kelola Inventaris
│   ├── chat/              # Percakapan & Notifikasi Realtime
│   └── profile/           # Profil Pengguna, Riwayat Transaksi, Ulasan
├── app.dart               # Konfigurasi root widget & Router
└── main.dart              # Entry point aplikasi
```

---

## 🚀 Panduan Memulai (Getting Started)

### 1. Prasyarat Sistem
* [Flutter SDK](https://docs.flutter.dev/get-started/install) (versi `>= 3.20.0`)
* Android Studio / VS Code dengan ekstensi Flutter & Dart
* Emulator Android / iOS Simulator atau perangkat fisik aktif

### 2. Langkah Instalasi

1. **Clone repository:**
   ```bash
   git clone https://github.com/username/RentIT_MobileApp.git
   cd RentIT_MobileApp
   ```

2. **Pasang dependensi:**
   ```bash
   flutter pub get
   ```

3. **Setup Environment Variable (`.env`):**
   Buat file `.env` pada direktori root proyek:
   ```env
   SUPABASE_URL=https://your-project.supabase.co
   SUPABASE_ANON_KEY=your-anon-key
   GOOGLE_MAPS_API_KEY=your-google-maps-api-key
   STRIPE_PUBLISHABLE_KEY=your-stripe-publishable-key
   ```

4. **Jalankan Aplikasi:**
   ```bash
   flutter run
   ```

---

## 🗺️ Roadmap Proyek

- [x] Inisialisasi Repositori & Dokumentasi Arsitektur
- [ ] Setup Base Project Flutter & State Management
- [ ] Modul Autentikasi Pengguna & Profil (KYC)
- [ ] Modul Katalog, Filter Kategori, & Tampilan Peta
- [ ] Modul Tambah & Kelola Barang Sewaan
- [ ] Sistem Kalender & Alur Booking Sewa
- [ ] Integrasi In-App Chat Realtime
- [ ] Integrasi Payment Gateway & Sistem Deposit
- [ ] Fitur Foto Inspeksi Check-In/Check-Out & Serah Terima
- [ ] Testing, Optimasi Build, & Rilis (Play Store / App Store)

---

## 🤝 Kontribusi

Kontribusi selalu disambut dengan baik! Jika ingin berkontribusi:
1. Fork repository ini
2. Buat branch fitur baru (`git checkout -b feature/NamaFiturKeren`)
3. Lakukan commit perubahan (`git commit -m 'feat: Menambahkan fitur X'`)
4. Push branch ke repository (`git push origin feature/NamaFiturKeren`)
5. Buka **Pull Request**

---

## 📄 Lisensi

Proyek ini dilisensikan di bawah **MIT License** - lihat file [LICENSE](LICENSE) untuk detail selengkapnya.