# Pertemuan 06 Nested Loop Python


**Nama:** Azizah Nur Kholishah

**NIM:** 2225250116

**Kelas:** 3E

## Tujuan

Pada tugas ini saya belajar menggunakan nested loop pada Python. Nested loop digunakan untuk membuat tabel perkalian dari 1 sampai `n`. Selain itu, program juga digunakan untuk menghitung jumlah setiap baris, total semua hasil perkalian, dan banyaknya hasil perkalian yang genap.

## Cara Menjalankan

Program dijalankan melalui terminal VS Code dengan perintah:

```bash
python3 tugas/tabel_perkalian_dan_statistik.py
```

Setelah program dijalankan, masukkan nilai `n`. Nilai `n` harus lebih dari 0. Jika memasukkan nilai 0 atau negatif, program akan meminta input kembali.

## Algoritma Tugas 3

1. Masukkan nilai `n`.
2. Jika `n <= 0`, masukkan nilai `n` kembali sampai valid.
3. Atur `total_semua` dan `count_genap` menjadi 0.
4. Gunakan loop luar untuk menentukan nilai `i` dari 1 sampai `n`.
5. Atur `total_baris` menjadi 0 pada setiap baris.
6. Gunakan loop dalam untuk menentukan nilai `j` dari 1 sampai `n`.
7. Hitung `hasil = i * j`.
8. Tampilkan hasil perkalian.
9. Tambahkan hasil ke `total_baris` dan `total_semua`.
10. Jika hasil perkalian genap, tambahkan `count_genap`.
11. Setelah satu baris selesai, tampilkan jumlah baris tersebut.
12. Setelah semua baris selesai, tampilkan jumlah pasangan, total semua hasil, dan banyak hasil genap.

**Peran dalam program:**

* Loop luar digunakan untuk membuat baris.
* Loop dalam digunakan untuk membuat kolom dan menghitung `i * j`.
* `total_baris` digunakan untuk menjumlahkan hasil pada satu baris.
* `total_semua` digunakan untuk menjumlahkan semua hasil perkalian.
* `count_genap` digunakan untuk menghitung banyak hasil perkalian yang genap.

## Hasil Pengujian

| No. | Input | Hasil yang Diharapkan               | Keluaran Aktual                     |  Status  |
| --: | --------: | ----------------------------------- | ----------------------------------- | :------: |
|   1 | n = 1 | Pasangan = 1, Total = 1, Genap = 0  | Pasangan = 1, Total = 1, Genap = 0  | Berhasil |
|   2 | n = 2 | Pasangan = 4, Total = 9, Genap = 3  | Pasangan = 4, Total = 9, Genap = 3  | Berhasil |
|   3 | n = 3 | Pasangan = 9, Total = 36, Genap = 5 | Pasangan = 9, Total = 36, Genap = 5 | Berhasil |

## Analisis Efisiensi

Loop luar berjalan sebanyak `n` kali dan loop dalam juga berjalan sebanyak `n` kali. Jadi, loop dalam secara keseluruhan berjalan sebanyak `n × n` atau `n²` kali.

Dengan begitu, semakin besar nilai `n`, semakin banyak proses yang dilakukan. Kompleksitas waktunya adalah **O(n²)**.

## Refleksi

Saat mengerjakan program ini, kesalahan yang saya temukan adalah masalah indentasi pada nested loop. Loop dalam harus berada di dalam loop luar. Kalau indentasinya salah, program bisa error atau hasilnya tidak sesuai. Setelah indentasinya diperbaiki, program dapat berjalan sesuai yang diharapkan.
