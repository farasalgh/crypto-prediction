# Crypto Price Prediction

Proyek ini bertujuan untuk memprediksi harga cryptocurrency (contoh: Bitcoin) selama 7 hari ke depan menggunakan data historis dari API CryptoCompare dan model machine learning sederhana (Random Forest).

---

## Fitur Proyek
- Mengambil data harga historis cryptocurrency menggunakan API CryptoCompare.
- Membuat fitur tambahan seperti rata-rata bergerak (Moving Average).
- Melatih model machine learning untuk prediksi harga.
- Memprediksi harga cryptocurrency selama 7 hari ke depan.
- Visualisasi data historis dan hasil prediksi.

---

## Persyaratan
Sebelum menjalankan proyek ini, pastikan Anda memiliki:
1. **Python 3.7 atau lebih baru**.
2. **Pustaka Python berikut**:
   - `pandas`
   - `numpy`
   - `matplotlib`
   - `seaborn`
   - `requests`
   - `scikit-learn`
3. **API Key dari CryptoCompare**:
   - Daftar di [CryptoCompare API](https://min-api.cryptocompare.com/) untuk mendapatkan kunci API gratis.

---

## Cara Menggunakan
Ikuti langkah-langkah berikut untuk menjalankan proyek ini:

### 1. Clone Repository
Clone repository ini ke komputer Anda:
```bash
git clone https://github.com/farasalgh/crypto-prediction.git
cd crypto-prediction
```

### 2. Buat Virtual Environment
Buat dan aktifkan virtual environment:
```bash
# Buat virtual environment
python -m venv venv

# Aktifkan virtual environment
# Windows
venv\Scripts\activate
# Mac/Linux
source venv/bin/activate
```

### 3. Instal Dependensi
Instal pustaka yang diperlukan:
```bash
pip install -r requirements.txt
```

### 4. Jalankan Jupyter Notebook
Jalankan Jupyter Notebook untuk memulai proyek:
```bash
jupyter notebook
```

---

## Struktur Proyek
Berikut adalah struktur folder proyek:
```
crypto-price-prediction/
│
├── crypto_prediction.ipynb   # Notebook utama untuk prediksi harga
├── README.md                 # Dokumentasi proyek
├── requirements.txt          # Daftar pustaka yang diperlukan
└── data/                     # Folder untuk menyimpan data (opsional)
```

---

## Penjelasan Proyek

### 1. Mengambil Data
Data harga historis cryptocurrency diambil menggunakan API CryptoCompare. Data ini mencakup harga pembukaan, penutupan, tertinggi, dan terendah untuk setiap hari.

### 2. Pra-pemrosesan Data
- Menambahkan fitur tambahan seperti rata-rata bergerak 7 hari (MA7) dan 30 hari (MA30).
- Menambahkan kolom target untuk memprediksi harga 7 hari ke depan.

### 3. Melatih Model
Model **Random Forest Regressor** digunakan untuk memprediksi harga berdasarkan fitur:
- Harga penutupan (close)
- Rata-rata bergerak 7 hari (MA7)
- Rata-rata bergerak 30 hari (MA30)

### 4. Prediksi 7 Hari ke Depan
Model digunakan untuk memprediksi harga cryptocurrency selama 7 hari ke depan berdasarkan data terbaru.

### 5. Visualisasi
- Grafik harga historis cryptocurrency.
- Grafik perbandingan antara harga aktual dan prediksi.

---

## Contoh Output
### Visualisasi Harga Historis
![Harga Historis](https://via.placeholder.com/800x400?text=Grafik+Harga+Historis)

### Prediksi Harga
Prediksi harga cryptocurrency selama 7 hari ke depan:
```bash
[84159.85, 85283.72, 84988.04, 85410.34, 84344.34, 85283.72, 84988.04]
```

---

## Catatan
- Proyek ini menggunakan model sederhana (**Random Forest**) untuk pembelajaran. Akurasi prediksi dapat ditingkatkan dengan menggunakan model yang lebih kompleks seperti **LSTM**.
- Harga cryptocurrency sangat volatil, sehingga prediksi mungkin tidak selalu akurat.

---

## Lisensi
Proyek ini dilisensikan di bawah lisensi **MIT**. Anda bebas menggunakan, memodifikasi, dan mendistribusikan proyek ini.

---

## Kontribusi
Jika Anda ingin berkontribusi pada proyek ini:

1. Fork repository ini.
2. Buat branch baru untuk perubahan Anda:
   ```bash
   git checkout -b fitur-baru
   ```
3. Commit perubahan Anda:
   ```bash
   git commit -m "Menambahkan fitur baru"
   ```
4. Push ke branch Anda:
   ```bash
   git push origin fitur-baru
   ```
5. Buat **Pull Request**.

---

Jika Anda memerlukan bantuan lebih lanjut, silakan hubungi saya! 😊
