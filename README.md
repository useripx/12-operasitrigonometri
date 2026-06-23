<div align="center">

# 📐 Kalkulator Operasi Trigonometri

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Platform](https://img.shields.io/badge/Platform-Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![Repo Size](https://img.shields.io/github/repo-size/useripx/12-OperasiTrigonometri?style=for-the-badge&color=blue)
![Version](https://img.shields.io/badge/Version-1.0-blue?style=for-the-badge)
![License](https://img.shields.io/badge/License-Free-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Selesai-brightgreen?style=for-the-badge)
![PyInstaller](https://img.shields.io/badge/Build-PyInstaller-orange?style=for-the-badge&logo=pyinstaller&logoColor=white)
![Semester](https://img.shields.io/badge/Semester-1-blueviolet?style=for-the-badge)

**Aplikasi CLI (Command Line Interface) untuk melakukan berbagai operasi perhitungan matematika trigonometri dengan mudah.**

*Dibuat oleh Yogi Ario — Proyek Semester 1*

---

</div>

## 📖 Deskripsi

**Kalkulator Operasi Trigonometri** adalah aplikasi sederhana berbasis terminal yang dibangun dengan Python untuk mempermudah operasi perhitungan trigonometri dasar. Program ini menggunakan modul `math` bawaan Python. Aplikasi ini memungkinkan pengguna untuk menghitung nilai Sinus (Sin), Kosinus (Cos), dan Tangen (Tan) baik dalam format Derajat maupun Radian. Selain itu, terdapat fitur parser soal trigonometri secara langsung dan konversi antara Derajat dan Radian.

## ✨ Fitur Utama

- 📐 **Sinus, Kosinus, Tangen** — Hitung nilai trigonometri dari suatu sudut.
- 🔄 **Konversi Satuan** — Mendukung input dalam satuan *Derajat* maupun *Radian*, serta dapat mengonversi dari Derajat ke Radian atau sebaliknya.
- 📝 **Input Soal Langsung** — Anda bisa langsung mengetikkan soal matematika seperti `sin(30)`, `cos(45)`, atau `tan(60)`.
- 🛡️ **Auto Admin Privilege (UAC)** — Meminta akses Administrator secara otomatis saat dieksekusi di OS Windows agar tidak terjadi isu perizinan.
- 💻 **Tersedia Executable** — Bisa dijalankan langsung melalui file `.exe` atau di-install melalui file `.msi` tanpa memerlukan instalasi interpreter Python.

## 📁 Struktur Proyek

```
12 operasitrigonometri/
├── trigono.py             # Source code utama berbasis Python
├── trigono.spec           # File konfigurasi build PyInstaller
├── img.ico                # Icon aplikasi
├── build/                 # File temporary dan cache proses build
└── dist/                  # Folder tempat file hasil build berada
    ├── trigono.exe        # Aplikasi standalone (Executable)
    ├── setup x64.msi      # Setup installer Windows 64-bit
    └── setup x86.msi      # Setup installer Windows 32-bit
```

## 🚀 Cara Menjalankan

### Opsi 1: Menjalankan File Python

Pastikan Python sudah terpasang. Karena program ini menggunakan modul bawaan (`math`, `sys`, `ctypes`), tidak perlu instalasi dependensi tambahan.

```bash
python trigono.py
```
*(Catatan: Jendela User Account Control (UAC) mungkin muncul untuk meminta izin Administrator saat program mulai berjalan).*

### Opsi 2: Menjalankan File Executable

Gunakan file `.exe` yang sudah disediakan jika Anda tidak menginstal Python:
- Buka folder `dist/`
- Klik ganda pada `trigono.exe`

### Opsi 3: Instalasi menggunakan MSI

Anda juga bisa melakukan instalasi permanen di komputer Anda dengan menggunakan file installer MSI:
- `dist/setup x64.msi` (Untuk arsitektur 64-bit)
- `dist/setup x86.msi` (Untuk arsitektur 32-bit)

### Opsi 4: Build Ulang Executable

Anda bisa mem-build ulang aplikasinya menggunakan `PyInstaller`:

```bash
pip install pyinstaller
pyinstaller trigono.spec
```

## 📸 Contoh Penggunaan

```text
=== Kalkulator Sederhana Trigonometri oleh Yogi Ario ===
=== Cara Menggunakan Kalkulator Trigonometri ===
1. Pilih operasi trigonometri yang ingin Anda hitung.
2. Ikuti petunjuk untuk memasukkan sudut.
3. Jika Anda memilih 'Masukkan soal trigonometri', masukkan soal trigonometri dalam format yang benar.
4. Hasil perhitungan akan ditampilkan beserta cara menghitungnya.
5. Anda dapat memilih untuk menghitung lagi atau keluar dari kalkulator.

Pilih operasi trigonometri:
1. Sin
2. Cos
3. Tan
4. Konversi Derajat ke Radian
5. Konversi Radian ke Derajat
6. Masukkan soal trigonometri
7. Keluar
Masukkan pilihan (1/2/3/4/5/6/7): 6
Masukkan soal trigonometri (contoh: sin(30), cos(45), tan(60)): sin(30)
Hasil dari sin(30) adalah: 0.49999999999999994
Cara menghitung: Menggunakan formula sin(30.0) = hasil

Tekan 1 untuk menghitung lagi atau enter untuk keluar:
```

## 🛠️ Teknologi

| Komponen      | Detail                                 |
|---------------|----------------------------------------|
| Bahasa        | Python 3.x                             |
| Modul         | `math`, `ctypes`, `sys` (Built-in)     |
| Build Tool    | PyInstaller                            |
| Keamanan      | UAC Elevation Privilege (Windows)      |
| Platform      | Windows                                |

## 👤 Author

**Yogi Ario**

---

<div align="center">

*Proyek Mata Kuliah — Semester 1 — Teknik Informatika UNP*

</div>
