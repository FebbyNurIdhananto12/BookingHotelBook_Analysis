# 📚 Studi Kasus: Booking Hotel Book

## 👥 Anggota Kelompok
1. Zulvikar Harist (202110370311033)
2. Febby Nur Idhananto (202110370311043)

---

## 📖 Pendahuluan

### 🔍 1. Pernyataan Masalah
Industri perhotelan menghadapi tantangan dalam memaksimalkan pendapatan dengan mengelola tarif harian rata-rata (ADR) dan alokasi tipe kamar. Mengetahui hubungan antara tipe kamar yang dialokasikan dengan ADR sangat penting untuk menentukan strategi harga yang optimal dan meningkatkan pengalaman pelanggan. Masalah ini menarik karena memberikan wawasan langsung kepada pengelola hotel untuk mengoptimalkan profitabilitas dan mengurangi kesalahan alokasi kamar.

### 📊 2. Data yang Digunakan
- **URL Dataset** dapat diakses melalui tautan berikut:
  - 🔗 [Download Dataset](https://www.dropbox.com/sh/qwdaldzkp8yrqwj/AADTj_WQcuKA0bsEeCKU__98a?dl=1)
- **Dataset** mencakup atribut seperti:
  - `adr` (tarif harian rata-rata)
  - `assigned_room_type` (tipe kamar yang dialokasikan)
  - `previous_bookings_not_canceled` (pemesanan sebelumnya yang tidak dibatalkan)
  - `reserved_room_type` (tipe kamar yang dipesan)
  - `booking_changes` (perubahan pemesanan)
  - `deposit_type` (jenis deposit)
  - `agent` (agen pemesanan)
  - dll.
- **Metodologi:**
  - 🔄 Pembersihan data untuk mengatasi nilai hilang, duplikasi, dan memastikan format konsisten.
  - 📈 Analisis eksploratif (EDA) untuk memahami distribusi ADR berdasarkan tipe kamar.
  - 🔗 Korelasi statistik untuk mengukur hubungan antara tipe kamar dan ADR.

### 🔬 3. Pendekatan/Teknik Analisis
- **Eksplorasi Data:**
  - Mengelompokkan data berdasarkan tipe kamar dan menghitung rata-rata ADR.
  - Menampilkan distribusi ADR untuk setiap tipe kamar menggunakan boxplot.
- **Analisis Korelasi:**
  - Mengonversi tipe kamar menjadi variabel numerik dan menghitung korelasi dengan ADR.
  - Korelasi ini membantu mengidentifikasi seberapa kuat hubungan antara tipe kamar dan ADR.

### 🎯 4. Analisis Membantu Pengelola Hotel & Konsumen
- **Manfaat bagi Pengelola Hotel:**
  - Memahami tipe kamar mana yang menghasilkan pendapatan tertinggi.
  - Menentukan strategi harga berbasis data untuk memaksimalkan ADR.
- **Manfaat bagi Konsumen:**
  - Pengelolaan tipe kamar yang lebih baik memastikan pengalaman menginap yang konsisten.
  - Pelanggan dapat mendapatkan nilai yang lebih baik berdasarkan harga dan tipe kamar.

---

## 📦 Package yang Diperlukan

### 🗂️ Deskripsi Dataset
- Dataset ini berasal dari Dropbox dan mencakup informasi tentang:
  - `ADR` (Average Daily Rate), tipe kamar yang dialokasikan, dan atribut lainnya.
- **Data dikumpulkan untuk:**
  - Menganalisis kinerja tipe kamar berdasarkan tarif harian rata-rata.

---

## 🛠️ Langkah-Langkah Pembersihan Data
1. 🚿 **Hapus nilai hilang** pada kolom penting (`country`, `agent`, `company`).
2. 🛠️ **Imputasi nilai hilang:**
   - Rata-rata untuk kolom numerik.
   - Modus untuk kolom kategorikal.
3. 📅 **Konversi kolom tanggal** (jika ada).
4. 🗑️ **Hapus duplikasi** untuk memastikan setiap data unik.

---

## 📊 Hasil Analisis Data

### 🔍 Distribusi ADR Berdasarkan Tipe Kamar
- Rata-rata ADR dihitung berdasarkan tipe kamar.
- Ditampilkan menggunakan boxplot untuk visualisasi distribusi.
- ![Gambar1](https://github.com/FebbyNurIdhananto12/BookingHotelBook_Analysis/blob/main/Gambar/AVG%20dan%20ROOM.png)
- #### Rata-rata ADR Berdasarkan Tipe Kamar
| Tipe Kamar | Rata-rata ADR |
|------------|---------------|
| A          | 120.50        |
| B          | 110.20        |
| C          | 105.30        |
| D          | 98.00         |
| E          | 92.50         |
| F          | 87.40         |
| G          | 80.00         |

### 🌍 Analisis Berdasarkan Negara
- Menemukan 10 negara dengan kontribusi ADR tertinggi.
- Visualisasi menggunakan bar chart.
- ![Gambar2](https://github.com/FebbyNurIdhananto12/BookingHotelBook_Analysis/blob/main/Gambar/AVG%20dan%20country.png)
- #### Top 10 Negara dengan ADR Tertinggi
| No | Negara | Rata-rata ADR |
|----|--------|---------------|
| 1  | CHN    | 129.00        |
| 2  | MEX    | 121.56        |
| 3  | IRL    | 98.00         |
| 4  | ROU    | 93.36         |
| 5  | BEL    | 89.00         |
| 6  | GBR    | 87.80         |
| 7  | ITA    | 66.29         |
| 8  | PRT    | 64.36         |
| 9  | DEU    | 60.87         |
| 10 | FRA    | 59.10         |

---

## 🚀 Kesimpulan
- **Untuk Pengelola Hotel:**
  - Data memberikan panduan dalam menentukan harga optimal per tipe kamar.
  - Strategi ini dapat meningkatkan pendapatan dan pengalaman pelanggan.
- **Untuk Konsumen:**
  - Pengelolaan tipe kamar yang lebih baik menciptakan pengalaman menginap yang lebih konsisten dan bernilai.

---

## Salam Hangat dari si Analiysis Zul and Bruh💡🌟
