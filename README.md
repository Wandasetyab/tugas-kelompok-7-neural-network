# Tugas Kelompok 7 Neural Network

Repository ini berisi dokumentasi dan kode sumber hasil tugas Kelompok 7 untuk mata kuliah **Praktik Machine Learning**. Proyek ini berfokus pada implementasi algoritma Deep Learning untuk mengenali wajah secara real-time dengan membandingkan efektivitas Neural Network sederhana dan *Convolutional Neural Network* (CNN).

## Anggota Kelompok 7
* **Sherly Novia Indriani** - (231001057)
* **Dinda Oktavia Pratiwi** - (231001026)
* **Ahsanul Ikram** - (231001077)
* **Wanda Setya Budi** - (231001008)

**Dosen Pengampu:** Herfandi, Ph.D.

---

## Deskripsi Proyek
Proyek ini mengeksplorasi alur kerja *Deep Learning* (DL Workflow) yang meliputi:
1.  **Preprocessing:** Face cropping, grayscale conversion, dan resizing.
2.  **Data Augmentation:** Mengatasi keterbatasan dataset dengan teknik rotasi, translasi, dan manipulasi kecerahan untuk meningkatkan akurasi model.
3.  **Model Building:** Penggunaan Keras `Sequential` API untuk membangun layer konvolusi (`Conv2D`), pooling (`MaxPool2D`), dan `Dense Layer`.
4.  **Real-time Inference:** Integrasi model `.h5` yang telah dilatih dengan OpenCV untuk deteksi dan pengenalan wajah melalui kamera.

---

## Alat dan Library
* **Bahasa:** Python 3.x
* **Library Utama:**
    * `Keras` & `TensorFlow` (Deep Learning Framework)
    * `OpenCV` (Image Processing & Webcam Access)
    * `Scikit-Learn` (Label Encoding & Metrics Report)
    * `NumPy` & `Matplotlib` (Data Manipulation & Visualization)
* **Editor:** VS Code / Jupyter Notebook

---

## Tahapan Implementasi
Berdasarkan file `2. Implementasi Neural Network.ipynb`, langkah-langkah praktik meliputi:

### 1. Eksperimen Simple Neural Network
Membangun model dasar untuk mengklasifikasikan dataset angka acak guna memahami fungsi aktivasi (`ReLU`, `Sigmoid`) dan optimizer (`Adam`).

### 2. Persiapan Dataset Wajah
* Menggunakan dataset LFW (*Labeled Faces in the Wild*).
* Melakukan augmentasi gambar (rotasi 5-10 derajat, pergeseran pixel, dan penyesuaian kontras).
* *Balancing data* untuk memastikan setiap kelas memiliki jumlah sampel yang adil (1000 sampel per kelas).

### 3. Arsitektur CNN
Penyusunan arsitektur CNN yang terdiri dari beberapa blok konvolusi untuk ekstraksi fitur otomatis, diikuti oleh *Fully Connected Layer* untuk klasifikasi akhir menggunakan fungsi `softmax`.

### 4. Evaluasi Model
Menganalisis performa melalui *Confusion Matrix* dan *Classification Report* (Precision, Recall, F1-Score) untuk memvalidasi kemampuan generalisasi model terhadap data baru.

---

## Video Presentasi
Penjelasan mendalam mengenai kodingan, teori Deep Learning yang digunakan, serta demonstrasi pengenalan wajah secara langsung dapat dilihat di:
👉 [https://youtu.be/pbAEQ0y0LgQ]

---

## Cara Menjalankan
1. Clone repository ini.
2. Pastikan lingkungan Python sudah terinstall library yang dibutuhkan:
   ```bash
   pip install tensorflow opencv-python scikit-learn matplotlib numpy
