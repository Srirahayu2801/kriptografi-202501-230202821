# Laporan Praktikum Kriptografi
Minggu ke-: 3
Topik: [02 Cryptosystem (Komponen, Enkripsi & Dekripsi, Simetris & Asimetris)]  
Nama: [Sri Rahayu]  
NIM: [230202821]  
Kelas: [5Ikrb]  

---

## 1. Tujuan

1. Mengidentifikasi komponen dasar kriptosistem (plaintext, ciphertext, kunci, algoritma).
2. Menggambarkan proses enkripsi dan dekripsi sederhana.
3. Mengklasifikasikan jenis kriptosistem (simetris dan asimetris).
---

## 2. Dasar Teori
(Ringkas teori relevan (cukup 2–3 paragraf). 
Jawab: Definisi Cipher Klasik
    Cipher klasik adalah metode enkripsi dan dekripsi yang digunakan secara luas sebelum era komputasi modern. Mereka membentuk dasar kriptografi awal dan umumnya dapat diimplementasikan hanya dengan pensil, kertas, atau alat mekanik sederhana. Secara fundamental, cipher klasik beroperasi melalui dua teknik utama: substitusi, di mana setiap unit teks biasa (biasanya huruf) diganti dengan unit lain (seperti pada Cipher Caesar atau Cipher Vigenère), dan transposisi, di mana urutan huruf-huruf teks biasa diacak atau disusun ulang tanpa mengubah hurufnya sendiri (seperti pada Cipher Kolom). Meskipun efektif untuk komunikasi rahasia selama berabad-abad, keamanan cipher klasik sangat bergantung pada kerahasiaan kunci; namun, sebagian besar mudah dipecahkan saat ini menggunakan analisis frekuensi dan kekuatan komputasi modern.

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
- Pertanyaan 1: Sebutkan komponen utama dalam sebuah kriptosistem.
Komponen utama dalam sebuah kriptosistem (sistem kriptografi) terdiri dari lima elemen kunci yang bekerja sama untuk mengamankan komunikasi data:

1.  Plaintext (Pesan Asli): Ini adalah data atau informasi yang dapat dibaca dan dimengerti oleh manusia sebelum proses penyandian dilakukan.
2. Ciphertext (Pesan Tersandi):Ini adalah hasil dari proses enkripsi; pesan dalam bentuk yang tidak dapat dibaca tanpa kunci yang benar.
3. Algoritma Kriptografi (Cipher): Ini adalah fungsi atau prosedur matematis yang digunakan untuk melakukan enkripsi (mengubah plaintext menjadi ciphertext) dan dekripsi (mengubah ciphertext kembali menjadi plaintext).
4. Kunci (Key): Ini adalah parameter rahasia (sering berupa deretan bit) yang dimasukkan ke dalam algoritma. Kunci adalah elemen terpenting yang menentukan hasil enkripsi dan dekripsi, dan keamanannya menjadi dasar keamanan seluruh sistem.
5. Proses Enkripsi dan Dekripsi: Ini adalah prosedur komputasi aktual untuk mengubah format pesan menggunakan algoritma dan kunci yang telah ditentukan.
- Pertanyaan 2: Apa kelebihan dan kelemahan sistem simetris dibandingkan asimetris?
Keuntungan dan kelemahan sistem kriptografi simetris dibandingkan dengan asimetris berpusat pada perbedaan mendasar dalam penggunaan kunci: Perbandingan Kunci Simetris vs. AsimetrisFiturKriptografi Simetris (Satu Kunci)Kriptografi Asimetris (Sepasang Kunci)Kelebihan (Pros)Kecepatan Tinggi: Sangat cepat dan efisien untuk mengenkripsi data dalam jumlah besar.Manajemen Kunci Aman: Menyelesaikan masalah distribusi kunci dan mendukung Tanda Tangan Digital.Kelemahan (Cons)Masalah Distribusi Kunci: Membutuhkan saluran aman untuk pertukaran kunci rahasia.Lambat: Jauh lebih lambat dan membutuhkan daya komputasi yang lebih besar.Keuntungan Utama Sistem SimetrisKeuntungan utama dari sistem simetris adalah kecepatannya. Karena hanya menggunakan satu kunci dan melibatkan operasi matematis yang lebih sederhana, algoritma seperti Advanced Encryption Standard (AES) dapat memproses data dalam jumlah besar (enkripsi massal) dengan sangat cepat, menjadikannya ideal untuk mengamankan hard drive atau sesi komunikasi data yang berkelanjutan.Kelemahan Utama Sistem AsimetrisKelemahan utama dari sistem asimetris adalah efisiensi komputasi yang rendah. Algoritma seperti RSA atau ECC melibatkan operasi bilangan prima dan perpangkatan yang kompleks, sehingga membutuhkan waktu pemrosesan yang jauh lebih lama dibandingkan sistem simetris. Oleh karena itu, sistem ini jarang digunakan untuk mengenkripsi seluruh konten pesan yang besar.Secara praktis, kedua sistem ini biasanya digunakan bersama-sama dalam sistem hibrida: Kriptografi asimetris yang lambat digunakan untuk secara aman mendistribusikan kunci sesi simetris, dan kemudian kriptografi simetris yang cepat digunakan untuk mengenkripsi data aktual.
- Pertanyaan 3: Mengapa distribusi kunci menjadi masalah utama dalam kriptografi simetris?
Komponen utama yang membentuk sebuah kriptosistem terdiri dari lima elemen esensial: Plaintext (pesan asli yang dapat dibaca), Ciphertext (pesan tersandi yang tidak dapat dimengerti), Algoritma Kriptografi (cipher atau fungsi matematis untuk transformasi), Kunci (key sebagai parameter rahasia yang mengontrol algoritma), dan Proses Enkripsi/Dekripsi (prosedur untuk mengubah pesan antara dua bentuknya). Dalam perbandingan, kriptografi simetris menawarkan kelebihan berupa kecepatan dan efisiensi yang luar biasa karena hanya menggunakan satu kunci untuk kedua proses, menjadikannya ideal untuk mengenkripsi data dalam jumlah besar. Namun, kelemahan terbesarnya adalah distribusi kunci. Sebaliknya, kriptografi asimetris yang menggunakan sepasang kunci (publik dan privat) memiliki kelebihan dalam manajemen kunci yang aman dan dukungan untuk tanda tangan digital, meskipun memiliki kelemahan berupa kecepatan yang jauh lebih lambat. Mengenai masalah distribusi kunci, ini menjadi perhatian utama dalam kriptografi simetris karena kunci rahasia yang sama harus didistribusikan melalui saluran yang sudah terjamin aman sebelum komunikasi dimulai; jika kunci disadap, semua data akan terekspos, dan masalah ini diperparah oleh skalabilitas buruk yang menuntut pengelolaan kunci dalam jumlah eksponensial seiring bertambahnya pengguna.
)
---

## 8. Kesimpulan

Cryptosystem adalah fondasi keamanan digital yang dirancang untuk mengamankan data, beroperasi melalui lima komponen utama: Plaintext, Ciphertext, Algoritma (Cipher), Kunci, serta prosedur Enkripsi dan Dekripsi. Kriptografi dibagi menjadi dua kategori utama: sistem simetris menggunakan satu kunci rahasia yang sama untuk kedua proses, unggul dalam kecepatan untuk enkripsi data massal, tetapi bermasalah dengan distribusi kunci yang aman. Sebaliknya, sistem asimetris menggunakan pasangan kunci (Publik dan Privat), unggul dalam manajemen kunci dan otentikasi, meskipun jauh lebih lambat. Oleh karena itu, kriptosistem modern menggunakan pendekatan hibrida, memanfaatkan keunggulan keamanan distribusi kunci asimetris untuk menukar kunci, dan kemudian beralih ke kecepatan enkripsi simetris untuk transmisi data aktual.
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
