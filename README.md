# Pengolahan Citra Digital - Minggu III: Transformasi Geometrik dan Interpolasi

Proyek ini merupakan implementasi tugas praktikum Minggu III untuk mata kuliah Pengolahan Citra Digital. Fokus utama proyek ini adalah penerapan transformasi geometrik dasar dan berbagai teknik interpolasi menggunakan Python dan OpenCV.

## Informasi Mahasiswa
- **Nama:** Muhammad Rafi Fatihul Ihsan
- **NIM:** 24343016
- **Sesi:** 202523430039

---

## Capaian Pembelajaran
Setelah mempelajari materi dalam proyek ini, diharapkan dapat:
1. Mengimplementasikan transformasi geometrik dasar: translasi, rotasi, dan scaling menggunakan matriks.
2. Menerapkan koordinat homogen untuk transformasi affine yang konsisten.
3. Membedakan dan mengimplementasikan teknik interpolasi: *nearest neighbor*, *bilinear*, dan *bicubic*.
4. Menganalisis perbedaan transformasi affine dan perspektif serta aplikasinya.
5. Mengevaluasi kualitas hasil transformasi menggunakan metrik PSNR dan MSE.
6. Merancang pipeline transformasi geometrik untuk aplikasi nyata.

## Struktur Proyek
Proyek ini terdiri dari dua komponen utama yang terletak di folder `src/`:

1.  **Praktikum**: Berisi demonstrasi teknik dasar transformasi geometrik (translasi, rotasi, scaling, shearing, affine, dan perspektif) serta perbandingan kualitas metode interpolasi menggunakan citra uji sintetis.
2.  **Assignment**: Implementasi pipeline transformasi geometrik untuk aplikasi registrasi citra menggunakan dua buah foto objek nyata dengan perspektif yang berbeda.

## Fitur Utama
- **Transformasi Geometrik**:
    - Berbasis matriks dan koordinat homogen.
    - Estimasi Transformasi Affine (minimal 3 titik).
    - Estimasi Transformasi Perspektif (minimal 4 titik).
- **Metode Interpolasi**:
    - *Nearest Neighbor* (INTER_NEAREST)
    - *Bilinear Interpolation* (INTER_LINEAR)
    - *Bicubic Interpolation* (INTER_CUBIC)
- **Metrik Evaluasi**:
    - **MSE** (Mean Squared Error)
    - **PSNR** (Peak Signal-to-Noise Ratio)
    - **Waktu Komputasi** (Estimasi efisiensi algoritma)

## Persyaratan Sistem
Pastikan Anda telah menginstal dependensi yang diperlukan sebelum menjalankan program:
```bash
pip install -r requirements.txt
```

Dependensi utama:
- `opencv-python`
- `numpy`
- `matplotlib`
- `scipy`

## Cara Menjalankan
1. Navigasi ke folder `src/praktikum/` dan jalankan `praktikum.py` untuk melihat demonstrasi dasar.
2. Buka file `src/assignment/assignment.ipynb` menggunakan Jupyter Notebook atau Google Colab untuk melihat implementasi pipeline registrasi citra pada objek nyata.

---
**Catatan**: File-file debug dan folder output bersifat lokal dan tidak disertakan sesuai dengan konfigurasi `.gitignore`.
