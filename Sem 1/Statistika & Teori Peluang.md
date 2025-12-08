# MATERI 1 - PRINSIP DASAR STATISTIKA DAN TEORI PELUANG

## Pengertian
- **`Sekumpulan angka untuk menerangkan sesuatu`**, baik angka yang belum tersusun (**`acak`**), maupun angka yang **`tersusun dalam suatu daftar atau grafik`**.
- Sekumpulan cara atau **`aturan tentang pengumpulan, pengolahan, analisis, serta penafsiran data`** yang  terdiri dari angka-angka.
- Sekumpulan **`angka yang menjelaskan sifat-sifat data atau hasil pengamatan`**.
- Cabang ilmu matematika yang mempelajarai **`cara (metode) pengumpulan, penyajian, analisis, intepretasi dan penarikan kesimpulan`** dari sekelompok data yang disusun dalam bentuk angka.

## Jenis Statistika
1. Statistika deskriptif: bagian statistika yang mempelajari cara **`pengumpulan dan penyajian data`** sehingga memberikan informasi yang berguna.
    - *central tendency (mean, median, modus)*
    - *variability (variance, std deviation, range, deviation, mean deviation, sum of squared deviation)*
    - *visualization (bar graph, histogram, table)*
2. Statistika inferensia: bagian statistika yang mencakup semua metode yang berhubungan dengan **`analisis`** sebagian data (sampel), sampai dengan **`penarikan kesimpulan`** mengenai keseluruhan data induk.
    - *estimation (z-scores)*
    - *random variable*
    - *parameter estimation*

## Data
Data merupakan karakteristik atau informasi, biasanya berupa angka, yang diperoleh melalui observasi. Data harus menggambarkan keterangan dari suatu keadaan.

## Sumber Data
- Primer (langsung dari narasumber)
    - wawancara
    - observasi
- Sekunder (dari pihak lain)
    - buku
    - jurnal
    - artikel
    - dokumen/publikasi lain

## Jenis Data
- Berdasarkan isi data
    - Kualitatif (data non-angka) [jenis kelamin, agama]
    - Kuantitatif (data angka) [umur, nilai, luas tanah]
- Berdasarkan luas data
    - Data diskrit (terbatas dan non-desimal, dari pencacahan) [jumlah penduduk]
    - Data kontinu (tdk terbatas, dari pengukuran) [tinggi, berat]

## Peluang 
Peluang merupakan ukuran kuantitatif mengenai kemungkinan suatu kejadian akan terjadi. (0-1) Teori peluang digunakan untuk memahami dan menghitung kejadian yang mengandung nilai acak.



# MATERI 2 - UKURAN PEMUSATAN DATA

## Data Tuggal

### Kuartil / Desil

$Q_i = X_{\frac{i(n+1)}{a}}$

- a = 4 untuk kuartil, 10 untuk desil
- i =  kuartil/desil yang dicari

## Data Berkelompok
| Nomor | xi   | Fi   | Fk   |
|-------|------|------|------|
| 1-9   | 5    | 2    | 2    |
| 10-19 | 15   | 4    | 6    |
| 20-29 | 25   | 6    | 12   |

### Mengubah data tunggal menjadi berkelompok
- Mencari jangkauan `J = Xmax - Xmin`
- Mencari banyak kelas (sturgess) `k = 1+3.3 log(n)` (bulatkan keatas)
- Mencari panjang kelas `C = J/k` (bulatkan keatas)

### Mean
Mean = $\frac{Σf_ix_i}{Σf_i}$
- $f_i$ = frekuensi
- $x_i$ = nilai tengah kelas
- $Σf_i$ = total frekuensi / Fk terakhir

### Median
Me = $T_B + \frac{(n/2) - F_k}{f_{Me}} C$

- $T_B$ = Tepi bawah (BB - 0.5)
- n = total data / frekuensi
- $F_k$ = frekuensi kumulatif sebelum
- $C = B_A - B_B + 1$

### Modus
$Mo = T_B + \frac{d_1}{d_1 + d_2} C$

- $d_1 = f_{i_{Mo}} - f_{i_{Mo-1}}$
- $d_2 = f_{i_{Mo}} - f_{i_{Mo+1}}$


### Kuartil / Desil
$Q_i = T_B + \frac{in/a - f_k}{f_{Q_i}} C$
- $f_{Q_i}$ = Frequency quartil/desil



# MATERI 3 - UKURAN PENYEBARAN DATA

## Range 
$X_{max} - X_{min}$

## Mean Deviation
$Md = \frac{Σ|X_i - Me|}{n}$

## Variance
$Σ^2 = \frac{Σ(X_i - Me)^2}{n}$ //untuk populasi

$s^2 = \frac{Σ(X_i - Me)^2}{n-1}$ //untuk sampel

## Standard Deviation
$Σ = s = \sqrt{\frac{Σ(X_i - Me)^2}{n-1}}$



# Materi 4 - PENYAJIAN DAN ANALISIS DATA

## Pengertian Data
- Data = bentuk jamak dari datum
- Data = keterangan-keterangan tentang suatu hal, dapat berupa sesuatu yang diketahui atau dianggap
    - Diketahui => pengamatan / percobaan
    - dianggap => perkiraan

## Pengumpulan Data
Proses pencatatan peristiwa atau karakteristik dari sebagian atau seluruh elemen populasi.

### Cara pengumpulan
- Pengamatan / observasi
- Studi literatur
- Kuisioner
- Wawancara / interview

### Banyaknya data yang diambil
- Sensus => pengumpulan data dari seluruh elemen populasi
- Sampel => pengumpulan data dari sebagian elemen populasi

## Pengolahan Data
Proses memperoleh data ringkasan dari data mentah dengan menggunakan cara / rumus tertentu.

## Penyajian Data
Agar mudah dapat lebih mudah dibaca dan dipahami

- Tabel
- Grafik
- Kartogram (grafik peta)

## Analisis Data
- Membandingkan dua hal / nilai variabel untuk mengetahui selisihnya (X-Y) atau rasionya (X/Y) kemudian menyimpulkan.
- Menguraikan / memecahkan keseluruhan menjadi komponen lebih kecil, sesuai tujuan analisis, agar dapat: 
    - Melihat ada tidaknya nilai ekstrem
    - Membandingkan antarbagian
    - Membandingkan antara bagian dan keseluruhan
- Memperkirakan / memperhitungkan besar pengaruh secara kuantitatif dari perubahan suatu kejadian terhadap suatu kejadian lainnya, kemudian meramalkannya.

# MATERI 5 - PROBABILITAS

## Ruang Sampel (S)
Adalah himpunan **`semua kemungkinan`** hasil dari suatu eksperimen acak

## Proses Pencacahan

### Enumerasi
memperoleh dan menghitung semua anggota ruang sampel

### Aturan Penjumlahan
Jika suatu prosedur terdiri dari *m* buah pekerjaan $T_1, T_2, ..., T_m$ dengan pekerjaan tersebut **`tidak bisa dikerjakan bersamaan`**, maka ada $n_1, n_2, ..., n_m$ cara untuk melakukan pekerjaan tersebut.

### Aturan Perkalian
Jika suatu prosedur terdiri dari *m* buah pekerjaan berurutan $T_1, T_2, ..., T_m$ dengan pekerjaan tersebut **`harus dilakukan secara bersamaan`**, maka ada $n_1, n_2, ..., n_m$ cara untuk melakukan pekerjaan tersebut.

### Permutasi
Jumlah cara penyusunan *r* objek dari *n* objek tanpa pengembalian **`dengan memperhatikan urutan`** penyusunannya.
- AAB != ABA
- $_nP_r = P(n, r) = \frac{n!}{(n-r)!}$
- Contoh: Kemungkinan pin atm 4 digit dengan tiap angka berbeda [$P(10, 4)$]

### Kombinasi
Jumlah cara penyusunan *r* objek dari *n* objek tanpa pengembalian **`TANPA memperhatikan urutan`** penyusunannya.
- AAB = ABA
- $_nC_r = C(n, r) = \frac{n!}{r!(n-r)!}$

## Teori Peluang
Besarnya kemungkinan suatu kejadian akan terjadi

### Sifat-Sifat
- Benilai antara 0-1
- Jumlah semua peluang kejadian di ruang sample harus sama dengan 1

### Persamaan Umum
$P(A) = \frac{n(A)}{n(S)}$

## Peluang Majemuk
Peluang dengan melibatkan 2 atau lebih kejadian

### Kejadian Saling Lepas (*Mutually Exclusive*)
Kedua kejadian tidak dapat terjadi pada waktu bersamaan
- $P(A \cup B) = P(A)+P(B)$
- $P(A \cap B) = P(\empty) = 0$

- Contoh: dadu dilempar, peluang muncul 1 atau 4.

### Kejadian Tak Saling Lepas
Kedua kejadian tersebut tidak dapat terpisah
- $P(A \cup B) = P(A)+P(B)-P(A \cap B)$
- $P(A \cap B) = P(A)+P(B)-P(A \cup B)$

- Contoh: 20% mahasiswa ambil matkul A dan 15% ambil B. Ada 5% mengulang keduanya. Kemungkinan mengambil salah satu.

### Kejadian Saling Komplementer
Kompelemen A adalah $\bar A$.  Komplementer A adalah yang bukan merupakan bagian dari A.
- P(A) + P($\bar A$) = P(S) = 1

- Contoh: Lempar 2 dadu bersamaan, peluang dapat angka berbeda. [$P(\bar A)$]

### Kejadian Saling Bebas
2 Kejadian yang mana kejadian pertama tidak mempengaruhi terjadinya kejadian kedua.

- Saling Lepas != Saling Bebas
- $P(A \cap B) = P(A)*P(B)$
- $P(A \cup B) = P(A)+P(B)$

- Contoh: Lempar 2 dadu bersamaan, peluang keluar angka 1 di keduanya.

### Kejadian Bersyarat
Jika kejadian A mempengaruhi kejadian B (atau sebaliknya)
- $P(A|B) = \frac{P(A \cap B)}{P(B)}$
- dgn syarat P(B) > 0
- B menjadi syarat A

# MATERI 6 - TEOREMA BAYES

## Law of Total Probability

Pada *n* buah kejadian sling lepas $A_1...A_n$, maka
- $P(B) = Σ{P(B|A_i)P(A)}$

dimana B adalah suatu peristiwa acak dan $P(B|A_i)$ adalah peluang B dengan syarat $A_i$

## Teorema Bayes
- menyatakan peluang terjadinya suatu peristiwa berdasarkan pengamatan sebelumnya yang mungkin relevan.
- bisa digunakan untuk menghitung P(B|A) berdasarkan informasi P(A|B) yang telah diketahui sebelumnya

- $P(A_i|B) = \frac{P(B|A_i)P(A_i)}{P(B)} = \frac{P(B|A_i)P(A_i)}{Σ{P(B|A_i)P(A_i)}}$

- $P(A_i)$ disebut peluang prior (nilai probabilitas awal yg diketahui sebelum ada info tambahan)
- $P(B)$ disebut peluang posterior (nilai peluang yang telah diperbaiki setelah mendapat infor tambahan)
- Contoh: 
    - Prior => Peluang terpilihnya angkatan 25
    - Posterior => Peluang terpilihnya angkatan 25 yg menyikai game


# MATERI 7 - REGRESI LINEAR
Regresi adalah alat ukur yang digunakan untuk mengetahui ada tidaknya korelasi antar variabel. 
Analisis regresi mempelajari bentuk hubungan antara 1 atau lebih variabel bebas dengan 1 variabel terikat

- Variabel Bebas (prediktor/*independent*) => sumbu X
- Variabel Tak Bebas (terikat/*dependent*) => sumbu Y

## Ukuran Dalam Regresi
- Koefisien Regresi (besarnya pengaruh X terhadap Y)
- Koefisien Korelasi (kuat tidaknya hubungan X dan Y)

## Pemahaman Regresi
Persamaan regresi memungkinkan peramalan nilai suatu variabel tak bebas dari nilai variabel bebas.

Garis regresi merupakan garis linear (hanya taksiran) yang menunjukan pola hubungan antara variabel, mis. X dan Y.

## Rumus Penting

| Kegunaan | Rumus |
| :------- | :--- |
| Persamaan Umum | $\hat y = a+bx$ |
| Slope (b) | $b = \frac{n Σ{xy}-Σ{x}Σ{y}}{nΣ{x^2}-(Σ{x})^2}$ |
| Slope (b) | $b = \frac{Σ(x_i-\bar x)(y_i-\bar y)}{Σ(x_i-\bar x)^2}$ |
| Intercept (a) | $a = \bar y - b \bar x$ |
| Residual (e) | $e_i = y_i-\hat y$ |
| SSE | $SSE = Σ{e^2}$ |
| SST | $SST = Σ{(y_i-\bar y)^2}$ |
| SSR | $SSR = SST-SSE$ |
| $R_2$ | $R_2 = 1-\frac{SSR}{SST}$ |
| Koef. Korelasi (r) [Pearson] | $r = \frac{n(Σxy)-(Σx)(Σy)}{\sqrt{[nΣx^2-(Σx)^2][nΣy^2-(Σy)^2]}}$ |
| Koef. Korelasi (𝜌) [Spearman] | $𝜌 = 1-\frac{6ΣD^2}{n(n^2-1)}$
| Variansi Residual ($s^2$) | $s^2 = \frac{SSE}{n-2}$ |
<!-- | Intercept (a) | $a = \frac{ΣyΣx^2-ΣxΣxy}{nΣ{x^2}-(Σ{x})^2}$ | -->


# MATERI 8 - REGRESI LINEAR BERGANDA
Mempelajari hubungan satu variabel terikat dengan beberapa variabel bebas.

- $y = b_0 + b_1x_1 + b_2x_2 + ... + b_nx_n$
- y = variabel terikat
- $x_1, x_2, ..., x_n$ = variabel bebas
- $b_0$ = konstanta
- $b_1, b_2, ..., b_n$ = koefisien regresi

## 2 Variabel
- $b_1 = \frac{Σx^2_2Σx_1y - Σx_1x_2Σx_2y}{Σx^2_1Σx^2_2-(Σx_1x_2)^2}$

## Semua
- $\hat b = (X^TX)^{-1}X^TY$

## Asumsi pada Regresi Linear Berganda

### Linearitas
Hubungan antara variabel bebas dan terikat bersifat linear (cenderung membentuk garis lurus)

### Homoskedastisitas
Variansi / sebaran dari error (selisih nilai sebenarnya dan prediksi) selalu konstan untuk semua tingkatan nilai di variabel bebas

Heteroskedastisitas adalah kebalikannya, menyebabkan model hanya mampu memprediksi akurat di nilai-nilai tertentu saja.

### Normalitas Residual
Residual (selisih nilai asli dan prediksi) seharusnya memiliki distribusi normal

### Multikolinearitas
- Terjadi ketika dua atau lebih variabel bebas memiliki korelasi yang tinggi
- Terdapat duplikasi informasi
- Jika variabel bebas (yg berkorelasi tinggi) berubah, model tidak bisa mengetahui variabel mana yang mempengaruhi variabel terikat
- Ex: Y => Harga rumah, $X_1$ => Luas tanah, $X_2$ => jumlah kamar (umumnya, luas tanah lebih besar berarti jumlah kamar lebih banyak) [korelasi tinggi]
