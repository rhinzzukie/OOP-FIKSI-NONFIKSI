# 📚 Sistem Perpustakaan Bu Sari
### *OOP-FIKSI-NONFIKSI — Tugas Pemrograman Berorientasi Objek*

---

## 📖 Deskripsi

Program simulasi **sistem peminjaman buku perpustakaan** berbasis Java yang menerapkan konsep-konsep dasar **Pemrograman Berorientasi Objek (OOP)**. Program ini memungkinkan pengguna untuk menambahkan buku (fiksi maupun non-fiksi), mendaftarkan anggota, dan mencatat peminjaman buku berdasarkan ISBN.

---

## ✨ Fitur

- ➕ Tambah buku **Fiksi** (dengan genre) dan **Non-Fiksi** (dengan topik)
- 👤 Daftarkan **anggota perpustakaan** dengan nama dan nomor KTP
- 🔍 Cari buku berdasarkan **ISBN**
- 📋 Tampilkan daftar semua buku dan anggota beserta pinjaman mereka
- ✅ Input interaktif via terminal menggunakan `Scanner`

---

## 🏗️ Struktur Kelas

```
Buku (abstract)
├── BukuFiksi
└── BukuNonFiksi

Anggota
Perpustakaan
Main
```

| Kelas | Deskripsi |
|---|---|
| `Buku` | Abstract class induk — menyimpan `judul` dan `isbn`, mendefinisikan method abstrak `displayInfo()` |
| `BukuFiksi` | Turunan `Buku` — menambahkan field `genre` |
| `BukuNonFiksi` | Turunan `Buku` — menambahkan field `topik` |
| `Anggota` | Menyimpan data anggota dan daftar buku yang dipinjam (`ArrayList`) |
| `Perpustakaan` | Mengelola koleksi buku dan anggota; menyediakan method pencarian buku |
| `Main` | Entry point program — menangani semua input/output pengguna |

---

## 🧠 Konsep OOP yang Diterapkan

| Konsep | Implementasi |
|---|---|
| **Abstraction** | Class `Buku` bersifat `abstract`, tidak bisa dibuat objeknya langsung |
| **Encapsulation** | Semua field menggunakan akses `private`, diakses lewat `getter` |
| **Inheritance** | `BukuFiksi` dan `BukuNonFiksi` mewarisi class `Buku` via `extends` |
| **Polymorphism** | Method `displayInfo()` di-*override* pada tiap subclass, dipanggil secara seragam lewat referensi `Buku` |

---

## 🚀 Cara Menjalankan

### Prasyarat
- Java Development Kit (JDK) 8 atau lebih baru
- Command Prompt / Terminal

### Langkah-langkah

```bash
# 1. Clone repository
git clone https://github.com/rhinzzukie/OOP-FIKSI-NONFIKSI.git
cd OOP-FIKSI-NONFIKSI

# 2. Compile semua file Java
javac *.java

# 3. Jalankan program
java Main
```

### Contoh Output

```
================================
SELAMAT DATANG DI TOKO BU SARI!!
SILAHKAN MAU PINJAM APA 
NANTI INGAT DIKEMBALIKAN YA
================================

Masukkan jumlah buku: 2

-- Buku ke-1 --
Jenis (1=Fiksi, 2=NonFiksi): 1
Judul : Harry Potter
ISBN  : 978-001
Genre : Fantasy

-- Buku ke-2 --
Jenis (1=Fiksi, 2=NonFiksi): 2
Judul : Belajar Java OOP
ISBN  : 978-002
Topik : Pemrograman
```

---

## 📁 Struktur File

```
OOP-FIKSI-NONFIKSI/
├── Buku.java
├── BukuFiksi.java
├── BukuNonFiksi.java
├── Anggota.java
├── Perpustakaan.java
└── Main.java
```

---

## 👨‍💻 Informasi

> Dibuat sebagai tugas mata kuliah **Pemrograman Berorientasi Objek**  
> Program Studi Ilmu Komputer — **Universitas Pendidikan Ganesha (Undiksha)**

---

*"Nanti ingat dikembalikan ya 📖"*
