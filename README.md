# Jupyter Notebook Code

Repo ini berisi dua notebook utama yang digunakan untuk membangun dan menguji model AI dalam mendeteksi serta memvalidasi pembuangan sampah.

---

## ✨ Tujuan Proyek
Membangun sistem AI untuk:
1. Mengklasifikasikan jenis sampah secara otomatis dari gambar.  
2. Memvalidasi perilaku pembuangan sampah melalui analisis video.

---

## 🚀 1. YOLO Trash Classification
**Notebook:** `yolo_trash_classification.ipynb`

### Deskripsi
Notebook ini digunakan untuk melatih model **YOLO (You Only Look Once)** agar mampu mengenali **jenis sampah dari gambar**.

### Alur Proses
- Load dataset gambar sampah
- Data augmentation untuk memperkaya variasi data
- Preprocessing label agar sesuai format YOLO
- Pembagian dataset: train, validation, dan test
- Training model YOLO
- Evaluasi performa model menggunakan metrik: **precision, recall, mAP**

### Output
Model terlatih untuk klasifikasi jenis sampah berdasarkan gambar.

---

## 🎥 2. Detection Video GIT
**Notebook:** `DetectionVideoGIT.ipynb`

### Deskripsi
Notebook ini digunakan untuk memvalidasi apakah sebuah **video pembuangan sampah dilakukan pada tempatnya** dengan memanfaatkan **model GIT (Generative Image-to-Text)**.

### Alur Proses
- Load video input
- Ekstraksi frame dari video
- Captioning tiap frame menggunakan model GIT
- Analisis deskripsi untuk menentukan apakah pembuangan sampah **sesuai** atau **tidak sesuai**

### Output
Kesimpulan video berupa status:
- ✅ Valid (Misi Berhasil)
- ❌ Tidak Valid (Misi Gagal)

---

## 📌 Catatan
- Dataset gambar sampah perlu disiapkan sebelum menjalankan `yolo_trash_classification.ipynb`.
- Untuk `DetectionVideoGIT.ipynb`, pastikan tersedia file video input dengan format `.mp4`.

---

## 👥 Tim Pengembang
- Monika
- Raihan Adi Pratama
- Vanessa Angelika

---

## 📜 by Trashvisor Team - SFT 2025