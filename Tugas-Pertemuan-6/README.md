# Program Perkalian Matriks 5 x 5

Reposotori ini dibuat untuk memenuhi tugas kuliah Bahasa Pemrograman II terkait implementasi sederhana dalam Python untuk melakukan **perkalian dua buah matriks berukuran 5 x 5**.

---

## Deskripsi Program

Matriks A dan Matriks B didefinisikan secara langsung dalam kode. Perkalian dilakukan dengan tiga perulangan yaitu `for-loop`, di mana setiap elemen hasil merupakan jumlah dari perkalian elemen baris Matriks A dan kolom Matriks B. Hasil akhirnya adalah matriks baru yang ditampilkan bersama Matriks A dan Matriks B.

---

## Source Code 
- Nilai matriks A 5x5
```python
matriksA = [
    [1, 2, 3, 4, 5],
    [0, 9, 8, 7, 6],
    [5, 6, 7, 8, 9],
    [6, 7, 8, 9, 0],
    [5, 4, 3, 2, 1]
]

matriksB = [
    [1, 1, 1, 1, 1],
    [1, 1, 1, 1, 1],
    [1, 1, 1, 1, 1],
    [1, 1, 1, 1, 1],
    [1, 1, 1, 1, 1]
]

# Proses perkalian matriks
hasil = []
for i in range(5):
    baris_hasil = []
    for j in range(5):
        total = 0
        for k in range(5):
            total += matriksA[i][k] * matriksB[k][j]
        baris_hasil.append(total)
    hasil.append(baris_hasil)
