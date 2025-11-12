# Laporan Praktikum Kriptografi
Minggu ke-: 5 
Topik: [Cipher Klasik (Caesar, Vigenère, Transposisi)]  
Nama: [Sri Rahayu]  
NIM: [230202821]  
Kelas: 5IKRB 

---

## 1. Tujuan
Setelah mengikuti praktikum ini, mahasiswa diharapkan mampu:  
1. Menerapkan algoritma **Caesar Cipher** untuk enkripsi dan dekripsi teks.  
2. Menerapkan algoritma **Vigenère Cipher** dengan variasi kunci.  
3. Mengimplementasikan algoritma transposisi sederhana.  
4. Menjelaskan kelemahan algoritma kriptografi klasik.  

---

## 2. Dasar Teori
---

Cipher Klasik merupakan teknik kriptografi awal yang digunakan untuk menyembunyikan pesan dengan cara mengubah bentuk teks asli (plaintext) menjadi teks sandi (ciphertext) menggunakan aturan tertentu. Tujuan utamanya adalah menjaga kerahasiaan informasi agar tidak dapat dibaca oleh pihak yang tidak berwenang. Cipher klasik terbagi menjadi dua jenis utama, yaitu cipher substitusi (mengganti huruf dengan huruf lain) dan cipher transposisi** (menukar posisi huruf tanpa mengubah bentuk hurufnya).

Caesar Cipher adalah salah satu jenis cipher substitusi paling sederhana, di mana setiap huruf pada plaintext digeser sejauh beberapa huruf dalam alfabet. Misalnya, dengan pergeseran 3, huruf A menjadi D, B menjadi E, dan seterusnya. Proses ini dapat dituliskan dengan rumus *C = (P + k) mod 26*, di mana *C* adalah ciphertext, *P* adalah plaintext, dan *k* adalah nilai pergeseran.

Vigenère Cipher** merupakan pengembangan dari Caesar Cipher dengan menggunakan kunci berupa kata. Setiap huruf kunci menentukan besar pergeseran untuk huruf plaintext yang bersesuaian, sehingga pola pergeseran menjadi lebih kompleks dan sulit dipecahkan. Sementara itu, Cipher Transposisi tidak mengganti huruf, tetapi mengubah urutannya berdasarkan pola tertentu (seperti kolom atau baris), sehingga pesan asli menjadi acak. Ketiga metode ini menjadi dasar penting dalam perkembangan kriptografi modern karena memperkenalkan konsep enkripsi, dekripsi, dan kunci rahasia.

---

## 3. Alat dan Bahan
(- Python 3.x  
- Visual Studio Code / editor lain  
- Git dan akun GitHub  
- Library tambahan (misalnya pycryptodome, jika diperlukan)  )

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
