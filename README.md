**Nama:** Sekar Wahyuningrum
**NIM:** 2225250095
**Kelas:** 3E

---

## Tujuan

Pada pertemuan ini, saya mempelajari penggunaan perulangan **`for`** dan **`while`** dalam Python untuk menyelesaikan berbagai permasalahan yang membutuhkan proses secara berulang atau iteratif.

---

## Struktur Folder

```text
pertemuan-05-perulangan-NIM/
│
├── README.md
├── .gitignore
│
├── latihan/
│   ├── 01_tabel_perkalian.py
│   ├── 02_jumlah_bilangan.py
│   ├── 03_validasi_input.py
│   └── 04_hitung_genap.py
│
└── kuis/
    └── kuis2_deret_aritmetika.py
```

---

## Cara Menjalankan Program

Pastikan **Python** sudah terinstall pada komputer.

### Menjalankan program latihan

Dengan perintah:

```bash
python latihan/01_tabel_perkalian.py
```

atau:

```bash
python3 latihan/01_tabel_perkalian.py
```

### Menjalankan program kuis

```bash
python kuis/kuis2_deret_aritmetika.py
```

---

## Materi yang Dipraktikkan

| No. | Materi                        | Keterangan                                                                    |
| --: | ----------------------------- | ----------------------------------------------------------------------------- |
|   1 | Perulangan `for`              | Digunakan untuk melakukan perulangan berdasarkan jumlah atau urutan tertentu. |
|   2 | Perulangan `while`            | Digunakan untuk melakukan perulangan selama kondisi tertentu terpenuhi.       |
|   3 | `range()`                     | Digunakan untuk menghasilkan urutan bilangan dalam perulangan.                |
|   4 | Validasi input                | Digunakan untuk memastikan data yang dimasukkan sesuai dengan ketentuan.      |
|   5 | Seleksi `if` dalam perulangan | Digunakan untuk menentukan kondisi tertentu selama proses perulangan.         |
|   6 | Akumulasi dan pencacahan      | Digunakan untuk menghitung jumlah atau banyaknya data selama perulangan.      |
|   7 | Deret aritmetika              | Digunakan untuk menghasilkan dan menghitung jumlah suatu deret aritmetika.    |

---

# Latihan

## 1. Tabel Perkalian

Program menerima sebuah bilangan bulat dan menampilkan hasil perkalian bilangan tersebut dari **1 sampai 10**.

### Test Case

| No. | Input (`n`) | Keterangan                                       |
| --: | ----------: | ------------------------------------------------ |
|   1 |           4 | Menampilkan tabel perkalian 4 dari 1 sampai 10.  |
|   2 |          -3 | Menampilkan tabel perkalian -3 dari 1 sampai 10. |

---

## 2. Jumlah Bilangan

Program menghitung jumlah bilangan dari **1 sampai `n`**.

### Test Case

| No. | Input (`n`) | Hasil |
| --: | ----------: | ----: |
|   1 |           1 |     1 |
|   2 |           5 |    15 |
|   3 |          10 |    55 |

### Perhitungan

* `n = 1` → `1`
* `n = 5` → `1 + 2 + 3 + 4 + 5 = 15`
* `n = 10` → `1 + 2 + 3 + ... + 10 = 55`

---

## 3. Validasi Input

Program meminta pengguna memasukkan **nilai ujian dari 0 sampai 100**.

Jika nilai yang dimasukkan tidak berada dalam rentang tersebut, program akan menolak input dan meminta pengguna memasukkan nilai kembali.

### Test Case

| No. | Input | Status                                     |
| --: | ----: | ------------------------------------------ |
|   1 |   120 | Ditolak karena lebih dari 100              |
|   2 |    -5 | Ditolak karena kurang dari 0               |
|   3 |    75 | Diterima karena berada dalam rentang 0–100 |

**Hasil:** Program menolak nilai `120` dan `-5`, kemudian menerima nilai `75`.

---

## 4. Menghitung Bilangan Genap

Program menghitung banyaknya bilangan genap dari **1 sampai `n`**.

### Test Case

| No. | Input (`n`) | Banyak Bilangan Genap |
| --: | ----------: | --------------------: |
|   1 |           1 |                     0 |
|   2 |           2 |                     1 |
|   3 |           5 |                     2 |
|   4 |          10 |                     5 |

Contoh untuk `n = 10`, bilangan genap yang ditemukan adalah:

`2, 4, 6, 8, 10`

Sehingga jumlah bilangan genap adalah **5**.

---

# Kuis 2 — Deret Aritmetika

Program menerima tiga input, yaitu:

1. **Suku pertama (`a`)**
2. **Beda (`d`)**
3. **Banyak suku (`n`)**

Program menggunakan **`while`** untuk melakukan validasi nilai `n` dan **`for`** untuk menghasilkan setiap suku serta menghitung jumlah deret.

## Test Case

| No. | Suku Pertama (`a`) | Beda (`d`) | Banyak Suku (`n`) | Suku            | Jumlah |
| --: | -----------------: | ---------: | ----------------: | --------------- | -----: |
|   1 |                  2 |          3 |                 5 | 2, 5, 8, 11, 14 |     40 |
|   2 |                 10 |         -2 |                 4 | 10, 8, 6, 4     |     28 |
|   3 |                1.5 |        0.5 |                 3 | 1.5, 2.0, 2.5   |    6.0 |

### Contoh Perhitungan

Untuk:

* `a = 2`
* `d = 3`
* `n = 5`

Deret yang dihasilkan:

`2, 5, 8, 11, 14`

Jumlah deret:

`2 + 5 + 8 + 11 + 14 = 40`

---

# Refleksi

Pada pertemuan ini, saya mempelajari penggunaan perulangan **`for`** dan **`while`** dalam Python untuk menyelesaikan permasalahan yang membutuhkan proses berulang.

Selain itu, saya juga mempelajari penggunaan **`range()`**, validasi input, seleksi **`if`** di dalam perulangan, serta teknik akumulasi dan pencacahan untuk memperoleh hasil dari proses perulangan.

Beberapa hal yang perlu diperhatikan dalam membuat perulangan adalah batas pada **`range()`**, pembaruan variabel kontrol pada **`while`**, dan penempatan variabel akumulator. Jika variabel kontrol pada perulangan **`while`** tidak diperbarui dengan benar, program dapat mengalami **infinite loop** atau perulangan yang tidak pernah berhenti.

---

# Hasil Pengujian

Seluruh program telah dijalankan menggunakan beberapa **test case** untuk memastikan bahwa:

* Perulangan berjalan sesuai dengan kondisi yang telah ditentukan.
* Perulangan berhenti pada kondisi yang benar.
* Validasi input dapat bekerja dengan baik.
* Perhitungan menghasilkan nilai yang sesuai dengan yang diharapkan.
* Program dapat menangani berbagai nilai input, termasuk bilangan positif, negatif, dan desimal pada kasus yang sesuai.

Berdasarkan hasil pengujian tersebut, program latihan dan kuis dapat menjalankan proses perulangan serta menghasilkan output sesuai dengan test case yang telah ditentukan.
