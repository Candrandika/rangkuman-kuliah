# 1. Sistem Bilangan

## Pengertian
Bilangan adalah suatu **`konsep matematika`** yang **`digunakan`** sebagai **`pencacah dan pengukuran`**. Simbol yang mewakili disebut **`angka`**.

## Jenis Bilangan
- Asli (N) => Bilangan bilangan positif >= 1
- Bulat
- Cacah => 0 + N
- Prima => bilangan yg hanya bisa dibagi oleh bilangan itu sendiri dan 1
- Komposit => >1, tapi bukan prima
- Pecahan => Bilangan yg dapat dinyatakan dalam bentuk a/b
    - a => pembilang, b => penyebut
    - b != 0
- Rasional => bilangan yg dapat dinyatakan dalam a/b
    - a dan b adalah bilangan bulat
    - b != 0
    - dapat ditulis sebagai desimal berhenti
- Irasional => bilangan yg tdk dapat dinyatakan dalam pecahan, atau pecahannya tidak berhenti seperti : $\sqrt{2}$, $\pi$
- Real => rasional + irasional

## Sifat Bilangan Real

### Sifat penjumlahan & pengurangan
- Asosiatif => $(a+b)+c = a+(b+c)$
- Komutatif => $a+b = b+a$
- Identitas => $a+0 = a$
- Invers => $a+(-a)=0$

### Sifat perkalian & pembagian
- Asosiatif => $(a*b)*c = a*(b*c)$
- Komutatif => $a*b = b*a$
- Invers => $a*(1/a) = 1$
- Distributif => $a*(b+c) = (a*b)+(a*c)$
- Identitas => $a*1 = a$

## Nilai Mutlak
Nilai mutlak dari suatu bilangan real $a$ adalah $|a|$, yang merupakan jarak bilangan tersebut ke titik-0.

### Sifat
- Non-negatif => $|a| \geq 0$
- Identitas => $|a| = 0$, jika dan hanya jika $a = 0$
- Simetri => $|a| = |-a|$
- Pertidaksamaan => $|a| \leq |-a|$ => $-b \leq a \leq b$

## Jenis Interval
| Simbol | Penjelasan        |
|:------:|:-----------------:|
| [a, b] | $a \leq x \leq b$ |
| (a, b) | $a < x < b$       |
| [a, b) | $a \leq x < b$    |
| (a, b] | $a < x \leq b$    |

## Contoh soal
1. Ubah $x = 0.136136...$ ke bentuk rasional
    - $1000x = 136.136...$
    - $x = 0.136...$
    - $1000x-x = 136.136...-0.136...$
    - $999x = 136$
    - $x = \frac{136}{999}$


# 2. Bentuk Persamaan dan Pertidaksamaan

## Pengertian
- Persamaan => pernyataan matematika yang menyatakan bahwa dua ekspresi matematika bernilai sama ($=$)
- Pertidaksamaan => pernyataan matematika yang menyatakan hubungan ketidaksetaraan antara dua ekspresi matematika ($<, >, \leq, \geq$)

## Jenis
| Jenis     | Penjelasan                                              | Bentuk Umum                                         |
|:---------:|:--------------------------------------------------------|:---------------------------------------------------:|
| Linear    | pangkat tertinggi variabelnya adalah 1                  | $ax+b = 0$                                          |
| Kuadrat   | pangkat tertinggi variabelnya adalah 2                  | $ax^2+bx+c = 0$                                     |
| Polinom   | lebih dari dua suku, masing2 dgn variabel pangkat bulat | $a_nx^n + a_{n-1}x^{n-1} + \ldots + a_1x + a_0 = 0$ |
| Rasional  | persamaan / pertidaksamaan dgn variabel dalam pecahan   | $P(x)/Q(x) = 0$                                     |
| Eksponen  | variabel sebagai eksponen                               | $a^x = b$                                           |
| Logaritma | melibatkan logaritma variabel                           | $log_a(x) = b$                                      |

# 4. Limit

## Pengertian
- Limit => nilai yang didekati oleh $f(x)$ saat $x$ mendekati $c$, tetapi tidak harus sama dengan $f(c)$
- $lim_{x \to a} f(x)$

## Aturan

- $lim_{x \to a} k = k$

- $lim_{x \to a} x = a$
- $lim_{x \to a} [f(x) ± g(x)] = $lim_{x \to a} f(x) ± lim_{x \to a} g(x)$
- $lim_{x \to a} [f(x) * g(x)] = $lim_{x \to a} f(x) * lim_{x \to a} g(x)$
- $lim_{x \to a} f(x)^n = [lim_{x \to a} f(x)]^n$

## Limit Trigonometri

- $lim_{x \to a} sin x = sin a$

- $lim_{x \to a} cos x = cos a$
- $lim_{x \to a} tan x = tan a$
- $lim_{x \to a} csc x = csc a$
- $lim_{x \to a} sec x = sec a$
- $lim_{x \to a} cot x = cot a$
- $lim_{x \to 0} \frac{sin x}{x} = 1$
- $lim_{x \to 0} \frac{1-cos x}{x} = 0$

## L'Hopital
- Hanya berlaku untuk limit tak tentu ($\frac{0}{0}$ atau $\frac{±\infty}{±\infty}$)
- Dilakukan dengan menurunkan pembuat 0 dari pembilang dan penyebut
- $lim_{x \to a} \frac{f(x)}{g(x)} = lim_{x \to a} \frac{f'(x)}{g'(x)}$


# Turunan

## Sifat-sifat
- $\frac{d}{dx}(x^n) = nx^{n-1}$
    - $\frac{d}{dx}(2x^4) = 8x^3$

- $(uv)`=u'v+uv'$
- $(\frac{u}{v})'=\frac{u'v-uv'}{v^2}$ 
- $f(g(x)) = f'(g(x))*g'(x)$
- $(f±g)'=f'±g'$
- $(a^x)' = a^xln(a)$
- $(lnx)' = 1/x$


# Integral

$\int x^n dx = \frac{1}{n+1}x^{n+1}+c$

## Sifat-sifat
= $\int k*f(x) dx = k*\int f(x) dx$
- $\int[f(x)±g(x)]dx = \int f(x)±\int g(x) dx$


# X. Trigonometri

## Koordinat Kartesius Vs Kutub

### Kartesius
- $A(x, y)$
- x => koordinat horizontal, y => koordinat vertikal

### Kutub
- $A(r, \alpha)$
- r => jarak radial, $\alpha$ => sudut

### Hubungan
- $x = r*\cos\alpha$
- $y = r*\sin\alpha$
- $r = \sqrt{x^2+y^2}$
- $\tan\alpha = y/x$

| Kartesius   | Kutub        |
|:-----------:|:------------:|
|$A(x_+,y_+)$ | $A(r,∠ K_1)$ |
|$A(x_-,y_+)$ | $A(r,∠ K_2)$ |
|$A(x_-,y_-)$ | $A(r,∠ K_3)$ |
|$A(x_+,y_-)$ | $A(r,∠ K_4)$ |

### Tabel trigonometri

| Sudut           | Sin   | Cos   | Tan   | Csc   | Sec   | Cot   |
|:---------------:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|
| **0°, 0**       | 0     | 1     | 0     | –     | 1     | –     |
| **30°, π/6**    | 1/2   | √3/2  | 1/√3  | 2     | 2/√3  | √3    |
| **45°, π/4**    | √2/2  | √2/2  | 1     | √2    | √2    | 1     |
| **60°, π/3**    | √3/2  | 1/2   | √3    | 2/√3  | 2     | 1/√3  |
| **90°, π/2**    | 1     | 0     | –     | 1     | –     | 0     |
| **120°, 2π/3**  | √3/2  | -1/2  | -√3   | 2/√3  | -2    | -1/√3 |
| **135°, 3π/4**  | √2/2  | -√2/2 | -1    | √2    | -√2   | -1    |
| **150°, 5π/6**  | 1/2   | -√3/2 | -1/√3 | 2     | -2/√3 | -√3   |
| **180°, π**     | 0     | -1    | 0     | –     | -1    | –     |
| **210°, 7π/6**  | -1/2  | -√3/2 | 1/√3  | -2    | -2/√3 | √3    |
| **225°, 5π/4**  | -√2/2 | -√2/2 | 1     | -√2   | -√2   | 1     |
| **240°, 4π/3**  | -√3/2 | -1/2  | √3    | -2/√3 | -2    | 1/√3  |
| **270°, 3π/2**  | -1    | 0     | –     | -1    | –     | 0     |
| **300°, 5π/3**  | -√3/2 | 1/2   | -√3   | -2/√3 | 2     | -1/√3 |
| **315°, 7π/4**  | -√2/2 | √2/2  | -1    | -√2   | √2    | -1    |
| **330°, 11π/6** | -1/2  | √3/2  | -1/√3 | -2    | 2/√3  | -√3   |
| **360°, 2π**    | 0     | 1     | 0     | –     | 1     | –     |

## Persamaan Penting

### Aturan
- $a/sinA = b/sinB = c/sinC$        (Aturan Sinus)
- $c² = a² + b² - 2ab*cosC$         (Aturan Cosinus)

## Sudut Rangkap
- $cos(2x) = 1-2sin^2x$

### Identitas
- $sin²θ + cos²θ = 1$
- $tanθ = sinθ / cosθ$
- $cotθ = cosθ / sinθ$
- $secθ = 1 / cosθ$
- $cscθ = 1 / sinθ$

### Penjumlahan pengurangan
- $sin(A ± B) = sinA cosB ± cosA sinB$
- $cos(A ± B) = cosA cosB ∓ sinA sinB$
- $tan(A ± B) = (tanA ± tanB) / (1 ∓ tanA tanB)$

