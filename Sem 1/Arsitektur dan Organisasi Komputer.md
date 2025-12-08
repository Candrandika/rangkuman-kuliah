# BAB 01 - KONSEP DASAR DAN EVOLUSI KOMPUTER

## Arsitektur dan Organisasi
| # | Arsitektur | Organisasi |
| - | - | - |
| Isi | apa yang dilakukan komputer | bagaimana komputer melakukannya |
| Definisi | Mengacu pada atribut yang *visible* untuk programmer. Memiliki dampak langsung pada eksekusi logis | Unit operasional dan interkoneksinya, yang mewujudkan spesifikasi arsitektural |
| Komponen | set instruksi, jumlah bit pada data, mekanisme I/O, teknik pengalamatan memori | Sinyal kontrol, interface antar komputer & peripheral, teknologi memori, clock. |
| Contoh | x86 / x64 |  Freq. processor, kapasitas cache, jenis RAM |
| Sifat | cenderung bertahan lama | cepat berubah seiring perkembangan teknologi |

## Struktur dan Fungsi
- Struktur => bagaimana tiap komponen saling berhubungan
- Fungsi => operasi dari tiap komponen sebagai bagian dari struktur

### Fungsi Dasar Komputer
- Data processing (pemrosesan data)
    - pengolahan data dari / ke memori
    - pengolahan data dari memori ke I/O
- Data storage (penyimpanan data)
    - short-term (memori volatile) [cache, RAM, register, virtual memory]
    - long-term (memori non-volatile) [hard disk, SSD, flash memory] 
- Data movement (perpindahan data)
    - pemindahan data dari peripheral ke perangkat lain
- Control (kontrol)
    - untuk pengaturan pada 3 fungsi lain
    - control unit -> bagian untuk mengelola sumber daya komputer dan mengatur kinerja bagian fungsional nya

### Struktur Komputer
- CPU => mengatur operasi komputer dan menjalankan fungsi pengolahan data
- Main memory => menyimpan data
- I/O => memindahkan data antara komputer dan lingkungan eksternal
- System interconnection / system bus => mekanisme komunikasinya

#### Struktur CPU
- Control Unit (CU) => mengatur pengoperasian CPU pada komputer
- Arithmetic and Logic Unit (ALU) => melakukan fungsi pengolahan data
- Registers => penyimpanan internal pada CPU
    - PC => iterasi => menyimpan instruksi yang akan dieksekusi
    - IR => meyimpan isi instruksi yg sedang dieksekusi
    - MAR => menyimpan addres yg akan diakses
    - MBR => menyimpan data yang baru dibaca
    - I/OAR => menyimpan address / id I/O yg akan dibaca
    - I/OBR => menyimpan data sementara yg ditukar antara CPU dan modul I/O
- CPU Interconnection => mekanisme komunikasi antara bagian-bagian CPU

## Evolusi Komputer

### Hukum Moore
**`Gordon Moore (cofounder Intel)`** pada **`1965`**, bahwa kerapatan komponen / **`jumlah transistor`** per chip **`meningkat 2x tiap tahunnya`**, dan **`menjadi tiap 1.5 tahun pada 1970`**.

- Konsekuensinya: 
    - harga tetap
    - kecepatan meningkat
    - ukurannya mengecil
    - penurunan daya

### Generasi Komponen
- Gen 1 (Vacuum Tubes) [1943-1953]
    - ENIAC 
    - IAS -> konsep stored-program (oleh John Von Neumann)
- Gen 2 (Transistor) [1947]
- Gen 3 (Integrated Circuit [IC]) [1958]
- Next Gen 
    - Large Scale Integration (LSI) -> > 1K komponen pada 1 chip IC
    - Veri Large Scale Integration (VLSI) -> > 10K komponen pada 1 chip IC
    - Ultra Large Scale Integration (ULSI) -> > 1B komponen pada 1 chip IC

### Semiconductor Memory
### Microprocessor 

## Komputer Modern

### Microprocessor VS Microcontroller
- Microprocessor => CPU dalam 1 chip
- Microcontroller => gabungan CPU, port I/O, memori, timer, dan lain yg jadi dikemas jadi 1 chip
- Microcontroller umumnya lebih lambat (MHz)
- Microcontroller tidak menyediakan interaksi dgn manusia

### Arsitektur

#### Intel x86
- berdesain CISC

#### ARM
- berdesain RISC untuk embeded system
- Chip berkecepatan tinggi, ukuran kecil, daya rendah
- banyak digunakan untuk perangkat genggam
- 3 Arsitektur
    - Cortex-A (A [32bit], A-50 [64bit])
        - Perangkat mobile
        - Mendukung MMU (Memory Management Unit)
        - Clock freq. tinggi
    - Cortex-R
        - Aplikasi real time
        - Mendukung MPU (Memory Protection Unit)
        - Clock freq. menengah
    - Cortext-M (M0, M0+, M3, M4)
        - IoT, wireless sensor
        - Mendukung MPU
        - Jumlah gerbang & konsumsi daya serendah mungkin




# BAB 02 - KINERJA DAN FUNGSI KOMPUTER TINGKAT ATAS

## Siklus Instruksi
Tiap siklus akan dimulai dari START, dan akan berakhir pada HALT.

### Siklus Dasar
- Fetch cycle
- Execute cycle
- Interupt cycle (cek -> ada ? jalankan)

### Siklus Utuh
- Instruction address calculation
- Instruction fetch
- Instruction decode
- Operand address calculation
- Operand fetch
- Data operation
- Operand store
- Check interupt

### Interupt
mekanisme yang membuat suatu modul dapat menginterupsi pengolahan normal prosesor

## Struktur Interkoneksi
Jalur komunikasi antara modul-modul dasar (memory, I/O, processor)

### Struktur transfer

- memory -> processor => baca instruksi / data
- processor -> memory => tulis data
- I/O -> processor => baca data via I/O module
- processor -> I/O => kirim data ke I/O device
- I/O <-> memory => Direct Memory Access

### Bus Interconnection Scheme
- Data Bus => memindahkan data -> lebarnya menentukan kinerja/kecepatan
- Address Bus => menentukan sumber/tujuan data bus -> lebarnya menentukan kapasitas memori maksimum
- Control Bus

### Quick Path Interconnect
Menggantikan bus bersama, menggunakan koneksi pairwase langsung dengan layered protocol architecture dan transfer data packetized untuk kinerja yang lebih tinggi dan latensi lebih rendah

### Peripheral Component Interconnect Express (PCIe)
Skema interkoneksi yang dirancang untuk menggantikan skema berbasis bus seperti PCI, dengan persyaratan kapasitas tinggi untuk perangkat I/O kecepatan tinggi.


## Peningkatan Kinerja Microprocessor
- Pipelining => memindahkan data/instruksi ke pipa konseptual 
- Branch Prediction => memprediksi instruksi
- Data flow analisys => menganalisis ketergantungan instruksi
- Speculative Instruction => (setelah BP / DFA) menjalankan instruksi secara spekulatif (dilakukan sebelum kemunculannya)

# BAB 03 - SISTEM BILANGAN DAN ARITMATIKA KOMPUTER

## Jenis Basis Bilangan
- Biner  => 0 dan 1
- Desimal => 0-9
- Octal => 0-7
- Hexadecimal => 0-9, A-F

## Konversi Bilangan Biner
- -> Desimal
    - $1011_2$ = 1*2^3 + 0*2^2 + 1*2^1 + 1*2^0 = $11_{10}$
- <- Desimal
    - $11_{10}$
        - 11/2 = 5 (sisa 1)
        - 5/2 = 2 (sisa 1)
        - 2/2 = 1 (sisa 0)
        - 1/2 = 0 (sisa 1)
    - $1011_2$ [dibalik]
- <-> Octal
    - $1110_2$ -> dibagi 3 bit
        - $001_2$ = $1_8$
        - $110_2$ = $6_8$
    - $16_8$
- <-> Hexa
    - $1110_2$ -> dibagi 4 bit
    - $E_{16}$




# BAB 04 - DIGITAL L0GIC

## Aljabar Boolean & Gerbang Logika

- AND => menghasilkan 1 jika kedua inputnya 1
- OR => menghasilkan 1 jika ada inputnya 1
- XOR => menghasilkan 1 jika inputnya berbeda
- NOT => membalikkan hasil




# BAB 05 - INTERNAL MEMORY

## Karakteristik Memori

### Lokasi
- Internal
- Eksternal

### Kapasitas 
- Kapasitas words
- Kapasitas bytes

### Unit transfer
- Word
- Block
- Internal memory unit transfer equal dengan number of electrical lines

### Metode akses
- Sequential -> data diakses berurutan. jika data ada diposisi 100, maka harus melewati posisi 1-99 terlebih dahulu (tape)
- Random -> langsung akses data sesuai dengan alamat yg dicari / diterima (RAM)
- Direct -> gabungan sequential dan random, data dibagi jadi block-block (HDD, CD)
- Associative -> pencarian langsung berdasarkan isi/data (cache)

### Performa 
- Access time => waktu yg dibutuhkan mulai dari CPU meminta hingga data tersaji
- Cycle time => waktu yg dibutuhkan untuk melakukan 1 cycle (awal - selesai operasi - memori siap menerima operasi selanjutnya)
- Transfer rate => kecepatan transfer data

### Tipe fisik 
- semiconductor
- magnetic
- optical
- magneto-optical

### Karakter fisik
- volatile/non-volatile
- erasable/non-erasable

### Organisasi [memory module]

## Hierarki Memori
- Register
- Cache (L1, L2, L3)
- Main memory
- Secondary memory

## Mapping Function
- Direct -> tiap blok memori utama dipetakan ke satu dan hanya satu line cache yang spesifik
- Associative -> blok memori dapat ditaruh di mana saja, tapi sirkuit cache harus mengecek semua baris sekaligus untuk menemukan label(tag) yang cocok
- Set Associative -> kombinasi direct dan associative

## Replacement Algorithm
- Least Recently Used (LRU) => data paling terakhir dipakai
- First-in-first-out (FIFO) => data yang masuk diawal, akan dibuang diawal juga
- Least Frequently Used (LFU) => data dgn freq. pemakaian paling jarang

## Semiconductor Memory Types
| Jenis | Kategori | Erasure | mekanisme | volatility |
| - | - | - | - | - |
| RAM | read-write | electrically, byte-level | electrical | volatile |
| ROM | read-ony | - | Masks | Non-volatile |
| PROM | read-only | - | Electrical | = |
| EPROM | read-mostly | UV light, chip-level | = | = |
| EEPROM | read-mostly | Electrically, byte-level | = | = |
| Flash Mem. | read-mostly | Electrically, block-level | = | = |

## RAM Technology
- Static RAM => menggunakan flip-flop (transistor yg saling mengunci) (cache)
- Dynamic RAM => menggunakan kapasitor untuk menyimpan data berupa muatan listrik (RAM)
    - Syncronous DRAM => DRAM yg memiliki clock syncronous dengan clock processor
    - Double Data Rate DRAM => SRAM tapi double
    - Rambus DRAM (RDRAM)
# BAB 06 - EXTERNAL MEMORY

## Magnetic Disk

Piringan budan dari substrat (kaca/aluminium) yang berlapis material megnetik

### R/W Mechanism

### Kinerja Disk
- Seek time => waktu memposisikan head ke track
- Rotational delay => waktu awal sektor meraih head pada track
- Access time => seek time + rotational delay
- Transfer time => waktu transfer data

### Bagian-Bagian
- Head => piringan budan yang bergerak
- Arm => piringan budan yang menggerakkan head
- Track => lingkaran pada piringan budan
- Sector => bagian-bagian dari track
- Spindle => poros penahan platter / piringan
- Cylinder => kumpulan semua track dalam posisi relatif sama dalam platter

### Layout
- CAV
    - jumlah sektor sama di tiap track, kepadatan berbeda di setiap track
- MZR

### Redundant Array of Independent Disk (RAID)
| Jenis | Jumlah disk |
| - | - |
| 0 | N |
| 1 | 2N |
| 2 | N+M |
| 3 | N+1 |
| 4 | N+1 |
| 5 | N+1 |
| 6 | N+2 |

## Solid State Drive

Menggunakan NAND flash memory

### Kelebihan & Kekurangan Dibanding HDD
- +IOPS tinggi
- +Daya tahan
- +Umur panjang
- +Daya rendah
- +Latency rendah
- -Kinerja menurun seiring penggunaan
- -batasan operasi write

## Magnetic Tape
- LTO


## Optical Memory
- CD (Compact Disk)
    - CD-ROM
    - CD-R
    - CD-RW
- DVD (Digital Versatile Disk)
    - DVD-R
    - DVD-RW
    - Blu-Ray DVD



# BAB 07 - INPUT/OUTPUT



# BAB 08 - OS



# BAB 09 - SET INSTRUKSI

|Mode|Notasi Simbol|Dimana Datanya?|Kecepatan|
| - | - | - | - |
Immediate | #5 | Di dalam instruksi | Paling Cepat |
Direct | [100] | Di Alamat 100 | Sedang |
Indirect | (100) | Di Alamat yang ditunjuk oleh isi Alamat 100 | Lambat (2x akses RAM) |
Register | R1 | Di Register R1 | Sangat Cepat |
Reg. Indirect | (R1) | Di RAM (alamatnya ada di R1) | Cepat |
Displacement | 10(R1) | Di RAM (alamat R1 + 10) | Cepat (Fleksibel) |
Stack | PUSH | Di Puncak Stack | Tergantung implementasi |