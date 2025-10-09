# Laporan Praktikum Kriptografi
Minggu ke-:1
Topik: CIA_intro.md  
Nama:  Sri Rahayu
NIM: 230202821  
Kelas: 5Ikrb  

Soal 1. Sejarah Singkat Kriptografi
Kriptografi, yang secara harfiah berarti "tulisan rahasia," bermula dari kebutuhan untuk menyembunyikan pesan.
1. Era Awal (Klasik)
Pada awalnya, kriptografi sangat sederhana. Contoh paling terkenal adalah Caesar Cipher, yang hanya menggeser huruf pada alfabet dengan jarak tetap. Teknik ini kemudian ditingkatkan dengan Vigenère Cipher, yang menggunakan kunci berupa kata sandi untuk membuat pola pergeseran yang berubah-ubah. Walaupun lebih kuat, metode klasik ini tetap rentan dan bisa dipecahkan dengan analisis statistik.
2. Revolusi Modern
Memasuki abad ke-20, kriptografi beralih ke ranah matematika dan komputasi. Inilah era kunci terbagi dua:
•	Kriptografi Kunci Simetris: Menggunakan kunci yang sama untuk enkripsi dan dekripsi. DES adalah standar awalnya, namun karena rentan, kini digantikan oleh AES (Advanced Encryption Standard), yang menjadi standar global karena efisiensi dan keamanannya.
•	Kriptografi Kunci Publik (Asimetris): Memungkinkan pengiriman pesan aman tanpa perlu bertukar kunci rahasia terlebih dahulu. Sistem pionirnya adalah RSA, yang mengandalkan bilangan prima besar untuk operasinya.
3. Era Digital Kontemporer
Saat ini, kriptografi adalah tulang punggung keamanan digital. Teknologi kunci publik telah melahirkan blockchain dan cryptocurrency (seperti Bitcoin). Di sini, fungsi hash kriptografis dan tanda tangan digital memastikan data transaksi sah, utuh, dan tidak dapat diubah. Perkembangan terbaru juga mencakup kriptografi kuantum dan zero-knowledge proof, yang fokus pada pengamanan data dari ancaman komputasi masa depan dan peningkatan privasi.
Singkatnya, kriptografi telah bertransformasi dari sekadar trik penyamaran menjadi disiplin ilmiah kompleks dan pondasi utama keamanan informasi di seluruh dunia digital.

Soal 2. Prinsip Keamanan Informasi CIA
a. Confidentiality (Kerahasiaan)
Pengertian:
Confidentiality berarti menjaga agar data atau informasi hanya dapat diakses oleh pihak yang berwenang. Tujuannya adalah melindungi data dari akses tidak sah, baik karena kesengajaan maupun kelalaian.
Contoh nyata:
Dalam sistem perbankan online, data seperti nomor rekening dan PIN nasabah dilindungi dengan enkripsi SSL/TLS, sehingga hanya pengguna dan server bank yang dapat membaca informasi tersebut.
Penggunaan autentikasi dua faktor (2FA) pada akun email juga menjaga kerahasiaan dengan memastikan hanya pemilik sah yang bisa login.
b. Integrity (Keutuhan)
Pengertian:
Integrity memastikan bahwa data tetap utuh, akurat, dan tidak diubah tanpa izin selama penyimpanan atau transmisi. Artinya, informasi yang diterima harus sama dengan yang dikirim, tanpa adanya manipulasi.
Contoh nyata:
Saat mengunduh file dari internet, sistem sering menyertakan checksum (hash MD5/SHA). Dengan membandingkan hash file yang diterima dan yang asli, pengguna dapat memastikan bahwa file tidak dimodifikasi oleh pihak ketiga.
Dalam transaksi keuangan, digital signature digunakan untuk menjamin bahwa isi pesan tidak diubah selama proses pengiriman.
c. Availability (Ketersediaan)
Pengertian:
Availability berarti memastikan bahwa sistem, data, dan layanan selalu dapat diakses oleh pengguna yang berwenang kapan pun dibutuhkan. Tujuannya adalah mencegah gangguan atau penolakan layanan.
Contoh nyata:
Situs e-commerce besar seperti Tokopedia atau Shopee menggunakan server redundan dan sistem backup agar tetap beroperasi meski terjadi gangguan atau serangan DDoS.
Dalam rumah sakit digital, server cadangan dan UPS (Uninterruptible Power Supply) digunakan agar sistem rekam medis tetap dapat diakses meskipun terjadi pemadaman listrik.

3.Apa perbedaan utama antara kriptografi klasik dan kriptografi modern ?
 Perbedaan utama anatara kriptografi klasik dan kriptografi modern terletak pada basis keamanan,kompleksitas, dan prinsip dasarnya. 
a.	Kriptografi klasik berfokus pada manipulasi karakter dan Bahasa menggunakan metode substitusi dan transposisi, dengan proses yang relatif sederhana dan dapat dilakukan secara manual. Keamanannya bergantung pada kerahasiaan algoritma yang digunakan.

b.	Kriptografi modern didasarkan pada matematika kompleks serta manipulasi data biner (bit), dan memerlukan komputer untuk melakukan perhitungan yang rumit. Prinsip keamanannya bergantung pada kerahasiaan kunci sesuai Prinsip Kerckhoffs, bukan pada algoritmanya. Selain itu, kriptografi modern memperkenalkan penggunaan kunci simetris seperti AES dan kunci asimetris/publik seperti RSA dan ECC, yang membuat sistemnya lebih aman dan efisien dibandingkan kriptografi klasik.