Hasil Praktik Big Data
BAB 6 Modul
Pada praktikum BAB 6 ini belajar tentang membuat modul. Python memiliki cara untuk menempatkan definis dalam file dan menggunakannya dalam skrip. File seperti itu disebut modul; definisi dari modul dapat diimpor ke modul lain atau ke dalam modul utama (kumpulan variabel yang Anda miliki akses ke skrip yang dijalankan di tingkat atas dan dalam mode kalkulator).

Modul adalah file yang berisi definisi dan pernyataan Python. Nama file adalah nama modul dengan akhiran .pyditambahkan. Dalam modul, nama modul (sebagai string) tersedia sebagai nilai variabel global name. Misalnya, gunakan editor teks favorit Anda untuk membuat file yang disebut fibo.pydi direktori saat ini dengan konten berikut:

Masukan interpreter Python dan impor modul ini dengan printah import fibo

Lebih lanjut tentang Modul Modul dapat berisi pernyataan yang dapat dieksekusi serta definisi fungsi. Pernyataan-pernyataan ini dimaksudkan untuk menginisialisasi modul. Mereka dieksekusi hanya saat pertama kali nama modul ditemukan dalam pernyataan impor.

Melaksanakan modul sebagai skrip Menjalankan modul Python dengan python fibo.py kode dalam modul akan dieksekusi, sama seperti jika Anda mengimpornya, tetapi dengan __name__set ke "main". Itu berarti bahwa dengan menambahkan kode ini di akhir modul Anda:

BAB 7 Input dan Output
Format String Literal -> string literal terformat memungkinkan untuk menyertakan nilai ekspresi Python di dalam string dengan mengawali string dengan f atau F menulis ekspresi sebagai {expression}
Format String() Metod -> penggunaan dasar dari str.format(). Contoh: print('{0} and {1}'.format('spam', 'eggs')). jika argumen kata kunci digunakan dalam str.format() metode, nilainya akan dirujuk dengan menggunakan nama argumen. Ini juga bisa dilakukan dengan melewatkan table sebagai argumen utama kunci dengan notasi.
Pemformatan String lama -> operator % juga dapat digunakan untuk string format.
Membaca dan menulis file -> open()mengembalikan file objek , dan ini paling sering digunakan dengan dua argumen: .open(filename, mode) f = open('workfile', 'w') Penjelasannya: Argumen pertama adalah string yang berisi nama file. Argumen kedua adalah string lain yang berisi karakter yang menjelaskan cara file akan digunakan. mode 'r' ketika file hanya akan dibaca, 'w' unuk hanya menulis, dan 'a' membukan file untuk menambahkan;
Metode Objek File ->
