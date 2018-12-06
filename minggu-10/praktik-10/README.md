Chapter 2: Essential DataFrame Operations
# Import Modul

import pandas as pd
import numpy as np
pd.options.display.max_columns = 40
Menampilkan beberapa kolom pada DataFrame
movie = pd.read_csv('data/movie.csv')
movie_actor_director = movie[['actor_1_name', 'actor_2_name', 'actor_3_name', 'director_name']]
movie_actor_director.head()
