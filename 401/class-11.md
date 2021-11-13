# numpy 

- Python data analysis package

- consisting of multidimensional array objects and a collection of routines for processing those arrays

- uses : 

    1- Mathematical and logical operations on arrays
    
    2- Fourier transforms and routines for shape manipulation.

    3- Operations related to linear algebra

- code

```
import numpy as np

np_arr = numpy.array(object, dtype = None, copy = True, order = None, subok = False, ndmin = 0)

np_arr.shepe() --> this gives the dimensions of the array

np_arr.reshape(x,y) --> this changes the dimension of the array

np_arr.itemsize () --> shows the size of its item type in the memory in bytes 

np.arrange(24) --> arranges value fron 0 to 23 as 1d arr 

np.empty(shape, dtype = float, order = 'C') --> create an empty

np.zeros(x,y) --> create a numpy array(matrix) of zeros

np.ones(x,y) --> create a numpy array(matrix) of ones

np.frombuffer(buffer, dtype = float, count = -1, offset = 0)

np.fromiter(iterable, dtype, count = -1)
np.arange(start, stop, step, dtype)

np.linspace(start, stop, num, endpoint, retstep, dtype) --> similar to arange() function. In this function, instead of step size, the number of evenly spaced values between the interval is specified.

numpy.logspace(start, stop, num, endpoint, base, dtype) --> returns an ndarray object that contains the numbers that are evenly spaced on a log scale. 



```
resorses 

[this](https://www.tutorialspoint.com/numpy/numpy_advanced_indexing.htm) totrial

[DataQuest](https://www.dataquest.io/blog/numpy-tutorial-python/)