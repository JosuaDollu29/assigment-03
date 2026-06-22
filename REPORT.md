# Buat Laporan Disini
# Laporan Tugas 2: Object-Oriented Programming (OOP) - SIM Akademik

## Data Diri
* **Nama:** Yosua Christian G Dollu
* **NRP:** 5024251077
* **Departemen:** Teknik Komputer

---

## 1. Penjelasan Struktur Program & Konsep OOP
Program ini mensimulasikan Sistem Informasi Manajemen (SIM) Akademik sederhana menggunakan paradigma Pemrograman Berorientasi Objek (OOP) di C++. Berikut adalah komponen dan konsep yang diterapkan:

* **Namespace (`sim`):** Digunakan untuk mengelompokkan seluruh class (`Orang`, `Mahasiswa`, `Dosen`, `Tendik`) agar menghindari konflik penamaan (*naming collision*) dan membuat kode lebih terstruktur.
* **Class `Orang` (Base Class):** Berperan sebagai kelas induk yang menyimpan data mendasar seperti `nama` dan `id`, serta fungsi `tampilkanInfoDasar()`.
* **Inheritance (Pewarisan):** * Class `Mahasiswa`, `Dosen`, `Tendik` merupakan kelas turunan (*derived class*) yang mewarisi atribut dan metode dari class `Orang`.
  * Masing-masing kelas turunan memiliki atribut spesifik (seperti `jurusan`, `spesialisasi`, atau `unitKerja`) dan metode uniknya sendiri (`belajar()`, `mengajar()`, `bekerja()`).

---

## 2. Struktur File Project
```text
assignment2-main/
├── src/
│   ├── include/
│   │   ├── orang.hpp
│   │   ├── mahasiswa.hpp
│   │   ├── dosen.hpp
│   │   └── tendik.hpp
│   ├── orang.cpp
│   ├── mahasiswa.cpp
│   ├── dosen.cpp
│   ├── tendik.cpp
│   └── main.cpp
└── REPORT.md
ketika progaram di jalankan memalui komplikasi manual g++
=== SIMULASI SISTEM INFORMASI MANAJEMEN AKADEMIK ===

Nama : Yosua Christian
ID   : 5024251077
Peran: Mahasiswa
Dept : Teknik Komputer
--------------------------
Yosua Christian sedang fokus belajar untuk perkuliahan.

Nama : Dr. Ir. Ahmad
ID   : 1985031201
Peran: Dosen
Bidang: Keamanan Siber
--------------------------
Dosen Dr. Ir. Ahmad sedang mengajar kelas Keamanan Siber.

Nama : Siti Maesaroh
ID   : 1990082403
Peran: Tenaga Kependidikan
Unit : Administrasi Akademik
--------------------------
Siti Maesaroh sedang mengurus administrasi di unit Administrasi Akademik.