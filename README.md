# TUGAS-2
# 📐 Latihan PBO: Implementasi Konsep OOP pada Bentuk Geometri

## Tentang Project

Project ini merupakan latihan mata kuliah Pemrograman Berorientasi Objek (PBO) menggunakan bahasa Java. Program dibuat untuk mempelajari penerapan konsep OOP melalui beberapa bentuk geometri, yaitu bentuk umum, bujur sangkar, lingkaran, dan silinder.

Setiap objek memiliki karakteristik masing-masing, seperti warna, panjang sisi, radius, dan tinggi. Program juga melakukan perhitungan luas dan volume sesuai jenis objeknya.

## 🛠️ Teknologi

- **Bahasa:** Java
- **Editor:** Visual Studio Code
- **Materi:** Object-Oriented Programming (OOP)

## 📁 File Program

| Nama File           | Kegunaan                                                     |
| ------------------- | ------------------------------------------------------------ |
| `Bentuk.java`       | Menyimpan atribut warna dan informasi dasar bentuk.          |
| `BujurSangkar.java` | Menghitung luas bujur sangkar.                               |
| `Lingkaran.java`    | Menghitung luas lingkaran berdasarkan radius.                |
| `Silinder.java`     | Menghitung volume silinder berdasarkan luas alas dan tinggi. |
| `Main.java`         | Membuat objek dan menjalankan program.                       |

## 📚 Pembahasan Materi

### 1. Encapsulation

Encapsulation diterapkan dengan membatasi akses langsung ke atribut menggunakan modifier `private`. Untuk mengambil atau mengubah nilainya, program menyediakan method getter dan setter.

Contohnya adalah atribut `warna`, `sisi`, `radius`, dan `tinggi`.

### 2. Inheritance

Inheritance memungkinkan sebuah class mewarisi fitur dari class lainnya. Dalam project ini, pewarisan diterapkan melalui kata kunci `extends`.

Struktur pewarisannya adalah:

- `BujurSangkar` merupakan turunan dari `Bentuk`.
- `Lingkaran` merupakan turunan dari `Bentuk`.
- `Silinder` merupakan turunan dari `Lingkaran`.

### 3. Polymorphism

Polymorphism ditunjukkan melalui method `printInfo()` yang dibuat ulang pada class turunannya menggunakan method overriding.

Setiap class memberikan keluaran yang berbeda. Bujur sangkar menampilkan luas, lingkaran menampilkan luas lingkaran, sedangkan silinder menampilkan volume.

### 4. Constructor

Constructor digunakan untuk menginisialisasi objek saat dibuat. Pada class turunan, `super()` digunakan untuk memanggil constructor milik class induk.

### 5. Perhitungan Geometri

Program menerapkan rumus berikut:

- **Luas bujur sangkar:** sisi × sisi
- **Luas lingkaran:** π × radius²
- **Volume silinder:** luas alas × tinggi

## 🚀 Langkah Menjalankan Program

Pastikan Java JDK sudah terpasang pada komputer.

1. Buka folder project menggunakan Visual Studio Code.

2. Buka terminal pada folder tersebut.

3. Compile seluruh file Java:

   ```bash
   javac *.java
   ```

4. Jalankan class utama:

   ```bash
   java Main
   ```

## 🖥️ Hasil Eksekusi

Contoh keluaran program:

```text
Bentuk berwarna Merah
BujurSangkar berwarna Biru, luas = 25.0
Lingkaran Hijau, luas = 153.86
Silinder warna Kuning, volume = 1538.6
```

Hasil dapat berbeda apabila nilai objek di dalam `Main.java` diubah.

## 📸 Dokumentasi Program

Screenshot berikut digunakan untuk menunjukkan hasil eksekusi program pada terminal.



---

**Kesimpulan**

Melalui latihan ini, konsep OOP dapat dipahami dengan membuat beberapa class yang saling berhubungan. Penggunaan encapsulation, inheritance, constructor, dan polymorphism membantu program menjadi lebih terstruktur dan mudah dikembangkan.
