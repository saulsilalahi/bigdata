Pengantar Struktur Data
DataFrame
DataFrame adalah struktur data tabular yang disusun pada kolom dan baris berurut. Untuk membuatnya lebih jelas, mari lihat contoh pembuatan sebuah DataFrame (tabel) dari kamus sebuah daftar.

Contoh berikut menunjukkan sebuah kamus berisi dua kunci, Name dan Age, dan daftar nilainya.

import pandas as pd
import numpy as np

name_age = {'Name' : ['Ali', 'Bill', 'David', 'Hany', 'Ibtisam'],
'Age' : [32, 55, 20, 43, 30]}
data_frame = pd.DataFrame(name_age)
print (data_frame)
hasil yang keluar seperti ini :



Series
Series adalah struktur data pandas kedua yang akan saya bicarakan. Series adalah object satu dimensi (1D) yang serupa dengan kolom di dalam tabel. Jika kita ingin membuat sebuah Series untuk daftar nama, kita dapat melakukan di bawah ini:

series = pd.Series(['Ali', 'Bill', 'David', 'Hany', 'Ibtisam'],
index = [1, 2, 3, 4, 5])
print (series)
hasil output :



Pelajaran 1
Create Data
contoh

names = ['Bob','Jessica','Mary','John','Mel']
births = [968, 155, 77, 578, 973]
untuk menggambungkan data bisa menggunakan perintah zip

zip

BabyDataSet = list(zip(names,births))
BabyDataSet
hasil yang di kerjakan :



seperti contoh dibawah ini df akan menjadi objek dataframe yang akan disimpan dengan format yang mirip seperti tabel sql :

df = pd.DataFrame(data = BabyDataSet, columns=['Names', 'Births'])
df
hasilnya :


Catatan
Direktori teori (biasanya) memuat rangkuman-rangkuman
Direktori praktik memuat penjelasan singkat mengenani kode sumber Python atau pustaka lain
