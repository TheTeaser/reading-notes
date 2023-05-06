# Read Topics: 11

## Jupyter Lab

1- **Multi-document interface:** Jupyter Lab provides a flexible and customizable interface that allows users to work with multiple documents and notebooks simultaneously. This means that you can open multiple notebooks, text editors, terminals, and other tools within a single Jupyter Lab instance.

2- **Integration with Git systems:** Jupyter Lab has built-in support for Git and other version control systems, which makes it easy to track changes, collaborate with others, and manage your code projects.

3- **Rich text editing:** Jupyter Lab provides a powerful rich text editor that supports Markdown, LaTeX, HTML, and other markup languages. This allows users to create documents that combine code, text, equations, and other media in a single notebook.

## Numpy Library

1- Create a multi-dimensional array.

2- Numpy provides a variety of Mathmatical functions support.

3- Using Numpe to read in files.

NumPy is  useful for scientific computing and data manipulation tasks because it provides a fast and efficient way to work with numerical data. The library is optimized for speed and performance.

The main data structure in NumPy is the ndarray, which is a shorthand name for N-dimensional array. 

an example on Numpy arrays:

```
import numpy as np

# create a 2D array
arr = np.array([[1, 2, 3], [4, 5, 6]])

# access array properties
print("Shape:", arr.shape)   # prints Shape: (2, 3)
print("Size:", arr.size)    # prints Size: 6
print("Data type:", arr.dtype)   # prints Data type: int64

# perform operations on arrays
arr_squared = arr ** 2
arr_sum = arr.sum(axis=0)

# broadcasting example
arr_broadcasted = arr + 1

# output results
print("Squared array:", arr_squared)
print("Column sums:", arr_sum)
print("Broadcasted array:", arr_broadcasted)
```