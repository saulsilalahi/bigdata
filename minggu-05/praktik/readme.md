OS Interface -> OS modul menyediakan puluhan fungsi untuk berinteraksi dengan sistem. Pastikan untuk menggunakan gaya daripada . Ini akan mencegah membayangi fungsi bawaan yang beroperasi jauh berbeda.import osfrom os import os.open() open()

File Wildcard -> Glob modul menyediakan fungsi untuk membuat daftar file dari pencarian direktori wildcard:

Argumen baris perintah -> Skrip utilitas umum sering perlu memproses argumen baris perintah. Argumen-argumen ini disimpan dalam atribut argvsys modul sebagai daftar. Sebagai contoh hasil keluaran berikut dari berjalan pada baris perintah:python demo.py one two three

Kesalahan output dan penghentian program -> sys Modul juga memiliki atribut untuk stdin , stdout , dan stderr . Yang terakhir ini berguna untuk memancarkan peringatan dan pesan kesalahan untuk membuatnya terlihat bahkan ketika stdout telah dialihkan:

Pencocokan pola string -> reModul menyediakan alat ekspresi reguler untuk pengolahan string yang canggih. Untuk pencocokan dan manipulasi yang kompleks, ekspresi reguler menawarkan solusi yang ringkas dan dioptimalkan:

Matematika -> modul math memberikan akses fungsi ke c library ** modul random digunakan untuk membuat pilihan acak ** modul statistik digunakan untuk menghitung sifat dasar statistik (mean, median, varian dll)

Akses Internet -> Dua modul untuk mengakses internet adalah urllib.request untk mengambil data dari URL dan smtplib untuk mengirim email:

Tanggal dan Waktu -> modul datetime digunakan untuk memanipulasi tanggal dan waktu dengan cara sedehana dan kompleks.

Kompresi Data -> pengarsipan data umum dan kompresi secara langsung didukun oleh modul termasuk : zlib, gzip, bz2, lzma, zipfile da tarfile.

Pengukuran kinerja ->

Kontrol Kualitas ->

Bab 10.1
osmodul menyediakan puluhan fungsi untuk berinteraksi dengan sistem operasi. Contoh

>>> import os
>>> os.getcwd()      # Return the current working directory
'C:\\Python37'
>>> os.chdir('/server/accesslogs')   # Change current working directory
>>> os.system('mkdir today')   # Run the command mkdir in the system shell
0
Built-in dir()dan help()fungsi berguna sebagai bantuan interaktif untuk bekerja dengan modul besar seperti os. Contoh

>>> import os
>>> dir(os)
<returns a list of all module functions>
>>> help(os)
<returns an extensive manual page created from the module's docstrings>
shutil modul ini menyediakan antarmuka tingkat yang lebih tinggi yang lebih mudah digunakan. Contoh

>>> import shutil
>>> shutil.copyfile('data.db', 'archive.db')
'archive.db'
>>> shutil.move('/build/executables', 'installdir')
'installdir'
Bab 10.2
glob modul menyediakan fungsi untuk membuat daftar file dari pencarian direktori wildcard. Contoh

>>> import glob
>>> glob.glob('*.py')
['wildcard.py', 'interfaceso.py']
Bab 10.3
Skrip utilitas umum sering perlu memproses argumen baris perintah. Argumen-argumen ini disimpan dalam atribut argvsys modul sebagai daftar.Contoh

>>> import sys
>>> print(sys.argv)
['demo.py', 'one', 'two', 'three']
Bab 10.4
sys Modul juga memiliki atribut untuk stdin , stdout , dan stderr . Yang terakhir ini berguna untuk memancarkan peringatan dan pesan kesalahan untuk membuatnya terlihat bahkan ketika stdout telah dialihkan. Contoh

>>> sys.stderr.write('Warning, log file not found starting a new one\n')
Warning, log file not found starting a new one
