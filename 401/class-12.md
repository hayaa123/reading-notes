# pandas 

```python
import numpy as np

import pandas as pd
```

- Series is a one-dimensional labeled array capable of holding any data type

```python 
s = pd.Series(data, index=index)
```

- DataFrame is a 2-dimensional labeled data structure with columns of potentially different types.

```python 
df = pd.DataFrame(data)
```
its kinds of data input

   Dict of 1D ndarrays, lists, dicts, or Series

   2-D numpy.ndarray

   Structured or record ndarray

   A Series

   Another DataFrame

## Dealing with DataFrame

pandas provides the `read_csv()` function to read data stored as a csv file into a pandas DataFrame.

```python
df = pd.read_csv("file_path.csv",index_col=0) # index_col=0 means let the first column of the data -> index 
df.head() #gives the top 5 rows of the data
df.plot() # plot the data in one line plot 
df.plo.hist() # plot histogram 
#other kind of plots 
plot_kind =['area',
 'bar',
 'barh',
 'box',
 'density',
 'hexbin',
 'hist',
 'kde',
 'line',
 'pie',
 'scatter']
pd.concat([df, df2], axis=0) # this will concatinate the tow data frames columns based in a common index
pd.concat([df, df2], axis=1) # this will concatinate the tow data frames rows based in a common rows 
```

resorses 

[Pandas in 10](https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html)

[Pandas - Getting Started](https://pandas.pydata.org/pandas-docs/stable/getting_started/intro_tutorials/index.html)

