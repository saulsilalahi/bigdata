Data Analysis di Pandas
Kode pada praktik in dapat langsung dilihat hasilnya melalui Jupyter Notebook

Berikut ini adalah kode sumber yang diambil dari buku dan dijadikan kode sumber terpisah per sub judul :

Data Analysis Routine
Reducing Memory by Changing Data Types
Selecting The Smallest of The Largest
Selecting The Largest of Each Group by Sorting
Replicating nlargest With sort_values
Calculating a Trailing Stop Order Price
Sebelum menjalankan kode perlu di impor dulu pustaka yang dibutuhkan

import pandas as pd
import numpy as np
from IPython.display import display
pd.options.display.max_columns = 50
Data Analysis Routine
Di sub bab ini akan menggunakan dataset college.csv yang terdapat di direktori data untuk kebutuhan analisis sederhana

college = pd.read_csv('data/college.csv')
print(college.head())
print(college.shape)

with pd.option_context('display.max_rows', 8):
    display(college.describe(include=[np.number]).T)

college.describe(include=[np.object, pd.Categorical]).T
print(college.info())

college.describe(include=[np.number]).T
college.describe(include=[np.object, pd.Categorical]).T

with pd.option_context('display.max_rows', 5):
    display(college.describe(include=[np.number], 
                 percentiles=[.01, .05, .10, .25, .5, .75, .9, .95, .99]).T)

college_dd = pd.read_csv('data/college_data_dictionary.csv')

with pd.option_context('display.max_rows', 8):
    display(college_dd)
