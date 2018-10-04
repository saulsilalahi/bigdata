Pertama buat file fibo.py di folder Python seperti contoh D:\python
di dalam file fibo.py , copy kan code berikut ini:

def fib(n): # write Fibonacci series up to n 
a, b = 0, 1 
while a < n: 
print(a, end=' ') 
a, b = b, a+b 
print() 
## 
def fib2(n): # return Fibonacci series up to n result = []<br> a, b = 0, 1<br> while a < n:<br> result.append(a)<br> a, b = b, a+b<br> return result` 

Setelah itu save di D:\python.
Kemudian di Python 3.7.exe jalankan code seperti di bawah: 

import sys
sys.path.append(r'D:\python')
import fibo

maka fibo selesai di import. Kemudian coba fibo tersebut dengan code dibawah : 

fibo.fib(1000)

Maka hasilnya seperti di samping : 0 1 1 2 3 5 8 13 21 34 55 89 144 233 377 610 987

6.1 More on Modules
import fibo as fib
fib.fib(500)

Maka hasilnya : 0 1 1 2 3 5 8 13 21 34 55 89 144 233 377

Maksud dari 'as' adalah inisialisasi nama file untuk mempersingkat code. 

6.2 Standard Modules
import sys
sys.ps1
'>>> '
sys.ps1 = 'C>'
C>print('Yeah!')
Yeah!
C>

Membuat sebuah perintah menuju directory C. 

6.3 The dir() Function
a = [1,2,3,4,5]
fib = fibo.fib
dir()
['__annotations__', '__builtins__', '__doc__', '__loader__', '__name__', '__package__', '__spec__', 'a', 'fib', 'fibo', 'sys']

Fungsi dir adalah fungsi mem-builtin apa saja yang sudah di built. 
