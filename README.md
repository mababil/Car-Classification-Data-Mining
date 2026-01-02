# 🚗 Klasifikasi Jenis Mobil

Project klasifikasi gambar mobil menggunakan CNN untuk mendeteksi 3 jenis mobil: **Bus**, **Pickup**, dan **Sport Car**.

---

## 📥 Download Project Lengkap

**Link Google Drive:** [Download di sini](https://drive.google.com/drive/folders/1fKSFqzfp9WelZGXwTYQxyNNtzJ0IKtKS?usp=drive_link)

> ⚠️ File model H5 dan assets tidak ada di GitHub karena terlalu besar. Download dari link di atas.

---

## 🚀 Cara Menjalankan

### 1. Setup Backend

```bash
cd backend
pip install flask tensorflow numpy pillow flask-cors
python app.py
```

Catat URL yang muncul, contoh: `http://127.0.0.1:5000`

### 2. Setup Frontend

Buka file `elegant_car_classification.html`, cari baris ini (sekitar line 900):

```javascript
url: 'http://127.0.0.1:5000/predict2',  // ← Ganti dengan URL backend Anda
```

Ganti sesuai URL backend yang tadi muncul, **jangan lupa tambahkan `/predict2`**

### 3. Jalankan

- Backend: Biarkan tetap jalan di terminal
- Frontend: Buka `elegant_car_classification.html` di browser

**Test:** Upload gambar mobil → Klik "CEK DATA" → Lihat hasil

---

## 🛠️ Troubleshooting

**Error "Terjadi kesalahan"?**
- Cek backend masih running
- Cek URL di HTML sudah benar
- Pastikan ada `/predict2` di akhir URL

**Gambar tidak muncul?**
- Pastikan folder `assets/` ada

---

## 💻 Tech Stack

- **Backend:** Flask + TensorFlow
- **Frontend:** HTML + CSS + JavaScript
- **Model:** CNN (Akurasi 96.7%)
