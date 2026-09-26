# Pertemuan 04 - Validasi Input dan Percabangan Bertingkat

## Identitas Mahasiswa

- Nama :Muhamad nurul bayan
- NIM :2225250115
- Kelas :3B

---

## Tujuan Pembelajaran

Pada praktikum ini mahasiswa diharapkan mampu:

1. Menggunakan percabangan bertingkat (`if`, `elif`, `else`) untuk pengambilan keputusan.
2. Melakukan validasi rentang nilai sebelum proses klasifikasi.
3. Melakukan validasi tipe data masukan pengguna.
4. Menggunakan operator logika dalam penyusunan kondisi.
5. Mengembangkan program sederhana yang memadukan validasi dan percabangan.

---

## Struktur Proyek

```text
pertemuan-04-validasi-NIM/
│
├── .gitignore
├── README.md
├── kuis.docx
│
├── latihan/
│   ├── 01_predikat_nilai.py
│   ├── 02_kategori_bilangan.py
│   ├── 03_validasi_rentang.py
│   ├── 04_validasi_tipe.py
│   └── 05_klasifikasi_segitiga_sudut.py
│
└── praktik/
    └── validasi_klasifikasi_nilai.py
```

---

## Cara Menjalankan Program

Pastikan Python sudah terinstal.

Jalankan program dengan perintah:

```bash
python nama_file.py
```

Contoh:

```bash
python latihan/01_predikat_nilai.py
```

---

# Latihan 1 - Predikat Nilai

## Deskripsi

Program menerima input nilai akhir (0–100) dan menentukan predikat nilai menggunakan percabangan bertingkat.

## Aturan Penilaian

| Nilai | Predikat |
| ------- | ------- |
| ≥ 85 | A |
| ≥ 70 | B |
| ≥ 60 | C |
| ≥ 50 | D |
| < 50 | E |

## Hasil Pengujian

| Input | Output |
| ------- | ------- |
| 90 | Predikat A |
| 75 | Predikat B |
| 65 | Predikat C |
| 55 | Predikat D |
| 40 | Predikat E |

---

# Latihan 2 - Kategori Bilangan

## Deskripsi

Program menerima sebuah bilangan bulat dan menentukan kategorinya.

## Kategori

- Bilangan negatif
- Nol
- Bilangan positif genap
- Bilangan positif ganjil

## Hasil Pengujian

| Input | Output |
| ------- | ------- |
| -5 | Bilangan negatif |
| 0 | Nol |
| 8 | Bilangan positif genap |
| 7 | Bilangan positif ganjil |

---

# Latihan 3 - Validasi Rentang

## Deskripsi

Program memvalidasi besar sudut sebelum menentukan jenis sudut.

## Aturan

- Sudut harus lebih dari 0°
- Sudut harus kurang dari 180°

## Hasil Pengujian

| Input | Output |
| ------- | ------- |
| 45 | Sudut lancip |
| 90 | Sudut siku-siku |
| 120 | Sudut tumpul |
| 180 | Masukan ditolak |

---

# Latihan 4 - Validasi Tipe

## Deskripsi

Program memvalidasi jumlah jawaban benar dari 20 soal kemudian menghitung persentase ketuntasan.

## Hasil Pengujian

| Input | Output |
| ------- | ------- |
| 15 | Persentase = 75%, Tuntas |
| 10 | Persentase = 50%, Belum Tuntas |
| abc | Masukan ditolak |

---

# Latihan 5 - Klasifikasi Segitiga Berdasarkan Sudut

## Deskripsi

Program menerima tiga sudut segitiga dan menentukan jenis segitiga setelah validasi.

## Aturan

- Semua sudut harus lebih dari 0°
- Jumlah ketiga sudut harus 180°

## Hasil Pengujian

| Input | Output |
| ------- | ------- |
| 60, 60, 60 | Segitiga lancip |
| 90, 45, 45 | Segitiga siku-siku |
| 120, 30, 30 | Segitiga tumpul |
| 100, 50, 20 | Masukan ditolak |

---

# Praktik - Validasi dan Klasifikasi Nilai Akhir

## Deskripsi

Program menggabungkan validasi input dan percabangan bertingkat untuk menentukan predikat serta status kelulusan mahasiswa.

## Rumus Nilai Akhir

```text
Nilai Akhir = (0.6 × Nilai Ujian) + (0.4 × Nilai Tugas)
```

## Ketentuan

- Kehadiran minimal 80%.
- Predikat A, B, dan C dinyatakan lulus.
- Predikat D dan E dinyatakan belum lulus.

## Tabel Keputusan

| Kondisi | Hasil |
| ------- | ------- |
| Kehadiran < 80% | Tidak memenuhi syarat |
| Nilai Akhir ≥ 85 | Predikat A |
| Nilai Akhir ≥ 70 | Predikat B |
| Nilai Akhir ≥ 60 | Predikat C |
| Nilai Akhir ≥ 50 | Predikat D |
| Nilai Akhir < 50 | Predikat E |

## Hasil Pengujian

| Nilai Ujian | Nilai Tugas | Kehadiran | Hasil |
| ------- | ------- | ------- | ------- |
| 90 | 80 | 90 | A, Lulus |
| 75 | 70 | 85 | B, Lulus |
| 65 | 60 | 90 | C, Lulus |
| 55 | 50 | 85 | D, Belum Lulus |
| 40 | 45 | 90 | E, Belum Lulus |
| 90 | 90 | 70 | Tidak memenuhi syarat kehadiran |

---

## Dokumentasi

Tambahkan screenshot hasil eksekusi program pada bagian ini.

---

## Refleksi

Pada praktikum ini saya mempelajari penggunaan validasi input dan percabangan bertingkat untuk menyelesaikan berbagai permasalahan logika. Saya memahami pentingnya memeriksa tipe data dan rentang nilai sebelum melakukan proses pengambilan keputusan sehingga program menjadi lebih aman dan sesuai dengan kebutuhan.