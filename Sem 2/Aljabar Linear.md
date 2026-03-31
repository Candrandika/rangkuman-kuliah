# PENGANTAR SISTEM PERSAMAAN LINEAR

## PERSAMAAN LINEAR
- Sebuah persamaan aljabar yang tiap sukunya mengandung konstanta atau perkalian konstanta dengan variabel tunggal
- Linear karena dapat digambarkan dalam garis lurus
- bentuk umumnya $y = mx + c$
    - $x$ = variabel
    - $m$ = koefisien
    - $c$ = konstanta

### Bentuk-bentuk persamaan linear
- bentuk umum => $a_1x_1 + a_2x_2 + ... + a_nx_n = b$
- homogen => $a_1x_1 + a_2x_2 + ... + a_nx_n = 0$
- 2d => $a_1x_1 + a_2x_2 = b$
- 3d => $a_1x_1 + a_2x_2 + a_3x_3 = b$

## SISTEM PERSAMAAN LINEAR
- Sekumpulan 2 atau lebih persamaan linear yang memiliki variabel sama dan harus diselesaikan secara bersamaan

### Bentuk umum
- $a_{11}x_1 + a_{12}x_2 + ... + a_{1n}x_n = b1$
- $a_{21}x_1 + a_{22}x_2 + ... + a_{2n}x_n = b2$
- ...
- $a_{m1}x_1 + a_{m2}x_2 + ... + a_{mn}x_n = bm$

dimana 
- $x_1, x_2, ..., x_n$ adalah variabel tidak diketahui
- $a_11, a_12, ..., a_1m$ adalah koefisien
- $b_1, b_2, ..., b_m$ adalah konstanta

### Solusi
SPL hanya memungkinkan terjadinya 3 macam solusi:
- tidak ada solusi (tidak semua garis bersinggungan pada 1 titik potong)
- 1 solusi (semua garis bersinggungan pada 1 titik potong)
- solusi tak hingga (semua garis berhimpitan)


# ELIMINASI GAUSS, MATRIKS DAN OPERASI MATRIKS, SIFAT-SIFAT MATRIKS

## AUGMENTED MATRIKS (Matriks diperbesar)

### Bentuk SPL
- $a_{11}x_1 + a_{12}x_2 + ... + a_{1n}x_n = b1$
- $a_{21}x_1 + a_{22}x_2 + ... + a_{2n}x_n = b2$
- ...
- $a_{m1}x_1 + a_{m2}x_2 + ... + a_{mn}x_n = bm$

### Bentuk Augmented Matiks
$
  \begin{bmatrix}
    a_{11} & a_{12} & ... & a_{1n} & b1 \\
    a_{21} & a_{22} & ... & a_{2n} & b2 \\
    ... & ... & ... & ... & ... \\
    a_{m1} & a_{m2} & ... & a_{mn} & bm
  \end{bmatrix}
$

## OPERASI BARIS ELEMENTER (OBE)

Metode dasar untuk menyelesaikan sistem linear adalah dengan melakukan operasi aljabar.

### Operasi Aljabar
- Perkalian / Pembagian ($R_1$ <- $2R_1$)
- Tukar posisi ($R_1$ <> $R_2$)
- Tambah konstanta ($R_1$ <- $R_1 + 2R_2$)

## BENTUK ECHELON

### Echelon
- Membentuk segitiga atas (bawah 0)
- Angka di bawah 1 utama harus 0

### Echelon Tereduksi
- Membentuk matriks identitas
- Angka di atas dan bawah 1 utama harus 0
- Menggunakan metode Gauss-Jordan

## METODE ELIMINASI

### GAUSS
- Menghasilkan echelon
- Tahap Forward

### GAUSS-JORDAN
- Menghasilkan echelon tereduksi
- Tahap Forward-Backward

## BENTUK SISTEM LINEAR HOMOGEN
- SPL disebut homogen jika konstantanya bernilai 0 semua
- Solusi semua $x$ nya adalah 0 (trivial)

# MATRIKS
- Array bilangan berbentuk persegi panjang
- Bilangan dalam matriks disebut elemen, entry, atau skalar
- Ukuran matrik adalah jumlah baris x kolom

## MATRIKS BUJUR SANGKAR / PERSEGI
Memiliki jumlah baris dan kolom yang sama

## DIAGONAL UTAMA
Diagonal utama ada pada tiap elemen dengan nomor kolom dan baris yang sama

## OPERASI MATRIKS

### Matriks Sama
Ketika matriks memiliki ukuran dan isi yang sama

### Penjumlahan dan Pengurangan Matriks
- Hanya bisa dilakukan saat memiliki ukuran yang sama.
- Dilakukan dengan menjumlahkan tiap pasang elemen

### Perkalian dengan Skalar
Mengalikan tiap elemennya dengan angka skalar

### Perkalian Matriks
- Hanya bisa dilakukan perkalian antara matriks $a×n$ dengan $n×b$
- Perhitungan dilakukan dengan menjumlahkan tiap hasil dari mengalikan baris dengan kolom

### Perkalian Matriks sebagai Kombinasi Linear
- Jika $A_1, A_2, ..., A_r$ adalah matriks yang memiliki ukuran sama
- Kemudian terdapat skalar $c_1, c_2, ..., c_r$
- Maka bentuk $c_1A_1 + c_2A_2 + ... + c_rA_r$ disebut kombinasi linear

### Transpose ($A^T$)
Melakukan penukaran elemen kolom menjadi elemen baris ($a_{ij}$ -> $a_{ji}$)

#### Sifat
- $(A^T)^T = A$
- $(A ± B)^T = A^T ± B^T$ 
- $(kA)^T = kA^T$
- $(AB)^T = B^TA^T$


### Trace ($Tr(A)$)
- Penjumlahan dari tiap elemen pada diagonal utama
- Hanya untuk matriks persegi

### Sifat-Sifat Matriks
- $A + B = B + A$ -> komutatif
- $A + (B + C) = (A + B) + C$ -> asosiatif
- $A(BC) = (AB)C$ -> asosiatif
- $A(B+C) = AB+AC$ -> distributif

- $A \pm 0 = A$
- $A - A = 0$
- $0A = 0$

Semua sifat jg berlaku untuk skalar

### Matriks Nol
Matriks dengan semua elemennya bernilai 0

### Matriks Identitas ($I$)
- Matriks dengan semua elemen diagonal utama 1, dan yg lain 0
- Hanya untuk matriks persegi

### Matriks Pangkat
- Hanya untuk matrik persegi
- $A^n = A×A×...×A $ (sebanyak n kali)
- $A^{-n} = A^{-1}×A^{-1}×...×A^{-1} $ (sebanyak n kali)

# INVERS MATRIKS ($A^{-1}$)
Matriks yang jika dikalikan dengan matriks asalnya akan menghasilkan matriks identitas
- matriks yang memiliki invers => matriks nonsingular / invertible
- matriks yang tidak memiliki invers => matriks singular

## Kegunaan
menyelesaikan spl, transformasi geometri, dll

## Sifat-Sifat
- $(A^{-1})^{-1} = A$
- $(A^{n})^{-1} = (A^{-1})^{n} = A^n$
- $(kA)^{-1} = k^{-1}A^{-1}$

## Menghitung Matriks Menggunakan Determinan

$
  \begin{bmatrix}
    a & b \\ c & d
  \end{bmatrix}
$

$det(A) = ad-bc$
$A^{-1} = \frac{1}{det(A)}
  \begin{bmatrix}
    d & -b \\ -c & a
  \end{bmatrix}
$

## Menghitung Invers menggunakan OBE (Operasi Baris Elementer) [Gauss-Jordan]

- $[A|I]$ -> $[I|A^{-1}]$


# DETERMINAN

## Pengertian

- Suatu fungsi yang mengaitkan setiap matriks persegi A berukuran $n*n$ dengan sebuah bilangan skalra
- Notasi: $det(A)$ atau $|A|$
- det: $\mathbb{R}^{n*n}$ -> $\mathbb{R}$ yang memetakan matriks persegi ke bilangan real

