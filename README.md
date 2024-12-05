# C242-PS030 Machine-Learning Path
Proudly presented by Capstone Team

# Table of Contents
1. [Introduction](#introduction)
2. [Components](#components)
3. [Requirements](#Requirements)
5. [Dataset](#dataset)
6. [Workflow](#workflow)
7. [Contributors](#contributor)



## Introduction Project
Fat Track is an AI-based application that helps users monitor their daily food content by recognizing images of food captured by the user and displaying the nutritional content of the food. Fat Track will display information such as calories, protein, fat, and carbohydrates of the food, which will then be stored to track the nutritional intake of the user's daily meals.

Theme : Healthcare


## Components
- Image Pre-processing
- Image Augmentation
- Early Stopping
- Callbacks
- Model Checkpoint
- Convolutional Neural Network (CNN)
- Transfer Learning
  - DenseNet121
  - InceptionV3
  - ResNet152V2
- Model Evaluation
- Accuracy and Loss Graph



## Requirements
| Library             | Version    |
|---------------------|------------|
| tensorflow          | 2.16.1     |
| keras               | 3.3.3      |
| matplotlib          | 3.7.5      |
| numpy               | 1.26.4     |
| pandas              | 2.2.3      |
| scikit-learn        | 1.2.2      |


## Dataset
File Dataset = https://drive.google.com/file/d/1B311xmZPac-LeUwJwfn-qODAzAbdSLAS/view?usp=drive_link




## Workflow
### 1. Download Gambar Menggunakan Bing Image Downloader
   - Gunakan **Bing Image Downloader** untuk mengunduh gambar makanan berdasarkan kategori (misalnya sate, rendang, nasi goreng).
   - Gambar akan disimpan dalam folder terstruktur sesuai dengan kategori makanan.

### 2. Open the .ipynb File in Google Colab or Jupyter Notebook
   - Buka file `.ipynb` di **Google Colab** atau **Jupyter Notebook**.
   - Pilih **File > Save a copy in Drive** untuk menyimpan salinan file ke akun Google Drive Anda. Ini akan memungkinkan Anda untuk mengedit dan menjalankan file notebook di Google Colab.

### 3. Preprocessing Data
   - Lakukan preprocessing pada gambar yang sudah diunduh:
     - **Cleaning**: Hapus gambar yang tidak relevan atau buram.
     - **Resizing**: Ubah ukuran gambar menjadi ukuran standar (misalnya 224x224 piksel).
     - **Normalisasi**: Skala piksel gambar menjadi rentang [0, 1].
     - **Augmentasi**: Terapkan augmentasi gambar seperti rotasi, flip, zoom, dll.

### 4. Model Building: Baseline Model (CNN)
   - Bangun model CNN dasar terlebih dahulu, untuk baseline, sebelum melanjutkan ke model yang lebih kompleks.

### 5. Transfer Learning Models
   - Implementasikan transfer learning menggunakan model pre-trained:
     - **DenseNet121**
     - **InceptionV3**
     - **ResNet152V2**
   - Tambahkan lapisan kustom jika perlu untuk menyesuaikan model dengan dataset Anda.

### 6. Training the Model
   - Latih model menggunakan data yang sudah diproses.
   - Gunakan **Early Stopping** untuk menghentikan pelatihan jika tidak ada peningkatan.
   - Simpan model terbaik menggunakan **Model Checkpoint**.

### 7. Run Every Cell in the .ipynb File
   - Jalankan setiap sel dalam file `.ipynb` untuk melatih model dan menghasilkan output yang diinginkan.
   - Pastikan bahwa proses berjalan tanpa error dan model dilatih dengan benar.

### 8. Model Evaluation
   - Evaluasi model menggunakan metrik yang relevan seperti:
     - Akurasi, Precision, Recall, dan F1-Score.
     - Visualisasi grafik akurasi dan loss selama pelatihan.

### 9. Download the Model .h5 File
   - Setelah model terlatih, **download model .h5** dengan mengklik file `.h5` di direktori Colab.
   - File model disimpan otomatis ke direktori `/content/` di Google Colab oleh **Model Checkpoint**.



## Contributor
| Name                       | Bangkit ID        | University                                |
|----------------------------|-------------------|-------------------------------------------|
| Ahmad Ferdiansyah           | M211B4KY0204      | Universitas Indraprasta PGRI              |
| Arif Adrian                 | M319B4KY0637      | Universitas Sumatera Utara                |
| Ikko Cahya Awinata          | M284B4KX1925      | Universitas Negeri Surabaya               |


