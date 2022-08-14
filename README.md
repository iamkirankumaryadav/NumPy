# `NumPy`

### **Why** to use NumPy ?
- Arithmetic, statistcal, mathematical, bitwise operations and linear algebra.
- Stacking, searching, sorting, counting, broadcasting and matrix operations.
- `Elementwise` arithmetic operations, `scientific` and `financial` calculations.
- `Array` processing, `N` dimensional array, fast `vector` and `matrix` operations.
- `Broadcasting` ( Arithmetic operations between array of different shape and size )
- Base for many other packages ( Pandas, SciPy, Statsmodel, Matplotlib, Scikit Learn )
- Essential for `OpenCV` computer vision applications ( Images pixels are converted into array )
- The datasets which are accepted by models for training are also in the form of array.

Attribute | Description
:--- | :---
`.shape` | 
`.size` |
`.ndim` | 

Method | Description
:--- | :---
`array()` | 
`arange()` | 
`unique()` |
`repeat()` |
`argmax()` | 
`argmin()` |
`reshape()` | 
`count_nonzero()` | 
`zeros()` | 
`ones()` | 
`ravel()` |
`hsplit()` | 
`vsplit()` | 
`hstack()` |
`vstack()` | 

[...](https://towardsdatascience.com/21-numpy-functions-that-will-boost-your-data-analysis-process-1671fb35215)

### **Similarities** between `Python Lists` and `NumPy Arrays`
- Both lists and arrays have similar syntax 
```python
# Python List
marks = [50, 45, 34]  

# NumPy Array
marks = np.array([50, 45, 34])
```
- Elements in both are `ordered`, `mutable` and accept `duplicates`
- Both allows `indexing`, `slicing` and `iterating`

### Python Lists Vs NumPy Arrays

**Python List** | **NumPy Array**
:--- | :---
No support for vectorized operations | Supports vectorized operations ( additions, multiplications )
Hold **Heterogeneous** / mixed data types | Hold **Homogeneous** data type
For loops are not efficient | For loops are fast and efficient
List is a default structure | Array needs import of NumPy library
Lists are flexible | Once the dimensions are defined cannot be expanded
Consumes more memory | Consumes 6x less memory
Slow ( During iteration data type of each element is checked ) | Faster ( All the elements are of same data type )

### Why NumPy array is faster than Python's list ?
- NumPy array elements only need memory to store element values.
- `List` stores much more information as compared to NumPy array.
- `List` stores `object type`, `reference count`, `object value` and `size` of value.
- Mathematical operations performed by Arrays are faster than Python's list.
 
```python
# Python List: Uses a for loop for just multiplying the elements with 5.
[i * 5 for i in list]

# NumPy Array: Simply multiplies each elements ( whole array ) with 5.
array * 5
```

<p align='right'><a align="right" href="https://github.com/KIRANKUMAR7296/Library/blob/main/Interview.md">Back to Questions</a></p>
