# Laporan Praktikum Kriptografi
Minggu ke-: 3
Topik: [03 Modular Math (Aritmetika Modular, GCD, Bilangan Prima, Logaritma Diskrit)]  
Nama: [Sri Rahayu]  
NIM: [230202821]  
Kelas: [5IKRB]  

---

## 1. Tujuan
Setelah mengikuti praktikum ini, mahasiswa diharapkan mampu:

1. Menyelesaikan operasi aritmetika modular.
2. Menentukan bilangan prima dan menghitung GCD (Greatest Common Divisor).
3. Menerapkan logaritma diskrit sederhana dalam simulasi kriptografi.

---

## 2. Dasar Teori
Cipher klasik adalah metode penyandian tradisional yang menggunakan algoritma sederhana untuk mengubah pesan asli (plaintext) menjadi pesan yang tidak bisa dimengerti (ciphertext) dengan tujuan menjaga kerahasiaan. Contoh cipher klasik adalah Caesar cipher, substitution cipher, dan transposition cipher, yang biasanya melibatkan penggantian atau penggeseran huruf sesuai aturan tertentu.

Aritmetika modular adalah konsep matematika yang berhubungan dengan bilangan bulat dan sisa pembagian terhadap suatu bilangan tetap yang disebut modulus. Dalam aritmetika modular, perhitungan dilakukan berdasarkan sisa hasil pembagian, sehingga hasilnya "berputar" kembali ke nol setelah mencapai nilai modulus tertentu. Dua bilangan dikatakan kongruen modulo n jika selisihnya merupakan kelipatan dari n. Konsep ini sangat penting dalam kriptografi, termasuk dalam cipher klasik, dimana misalnya huruf-huruf alfabet yang dipetakan ke angka 0 hingga 25 kemudian hasil operasi dijaga agar selalu dalam rentang angka tersebut menggunakan aritmetika modular.

---

## 3. Alat dan Bahan
(- Python 3.x  
- Visual Studio Code / editor lain  
- Git dan akun GitHub  

---

## 4. Langkah Percobaan
(Tuliskan langkah yang dilakukan sesuai instruksi.  
Contoh format:
1. Membuat file `caesar_cipher.py` di folder `praktikum/week2-cryptosystem/src/`.
2. Menyalin kode program dari panduan praktikum.
3. Menjalankan program dengan perintah `python caesar_cipher.py`.)

---

## 5. Source Code
(Salin kode program utama yang dibuat atau dimodifikasi.  
Gunakan blok kode:

```python
# contoh potongan kode
def encrypt(text, key):
    return ...
```
)

---

## 6. Hasil dan Pembahasan
(- Lampirkan screenshot hasil eksekusi program (taruh di folder `screenshots/`).  
- Berikan tabel atau ringkasan hasil uji jika diperlukan.  
- Jelaskan apakah hasil sesuai ekspektasi.  
- Bahas error (jika ada) dan solusinya. 

Hasil eksekusi program Caesar Cipher:

![Hasil Eksekusi](screenshots/output.png)
![Hasil Input](screenshots/input.png)
![Hasil Output](screenshots/output.png)
)

---

## 7. Jawaban Pertanyaan
(Jawab pertanyaan diskusi yang diberikan pada modul.  
- Pertanyaan 1: …  
- Pertanyaan 2: …  
)
---

## 8. Kesimpulan
(Tuliskan kesimpulan singkat (2–3 kalimat) berdasarkan percobaan.  )

---

## 9. Daftar Pustaka
(Cantumkan referensi yang digunakan.  
Contoh:  
- Katz, J., & Lindell, Y. *Introduction to Modern Cryptography*.  
- Stallings, W. *Cryptography and Network Security*.  )

---

## 10. Commit Log
(Tuliskan bukti commit Git yang relevan.  
Contoh:
```
commit abc12345
Author: Nama Mahasiswa <email>
Date:   2025-09-20

    week2-cryptosystem: implementasi Caesar Cipher dan laporan )
```
