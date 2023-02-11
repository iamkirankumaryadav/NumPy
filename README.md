# `NumPy`

- NumPy is foundation of other libraries like `Pandas`, `DataFrames` are build on NumPy arrays and can leverage NumPy functions.
- Only store a single data type (Mixed data type is stored as object | `string`)
- They can be one dimensional or multi dimensional.
- Array elements can be modified, but the array size cannot change.

### **Why** to use NumPy ?
- Arithmetic, statistcal, mathematical, bitwise operations and linear algebra.
- Stacking, searching, sorting, counting, broadcasting and matrix operations.
- `Elementwise` arithmetic operations, `scientific` and `financial` calculations.
- `N dimensional array` processing, fast `vector` and `matrix` operations.
- `Broadcasting` : Arithmetic operations between array of different shapes and size.
- `NumPy` is used as a base library for Pandas, SciPy, Statsmodel, Matplotlib, Scikit Learn.
- Essential for `OpenCV` computer vision applications ( Images pixels are converted into array )
- The datasets which are accepted by models for `fit` ( training | learning ) are also in the form of array.
- NumPy has a very rich set of [number generator](https://github.com/KIRANKUMAR7296/NumPy/blob/main/Number%20Generators.ipynb), [attributes](https://github.com/KIRANKUMAR7296/NumPy/blob/main/Attribute.md) and [methods](https://github.com/KIRANKUMAR7296/NumPy/blob/main/Method.md)

### `Array`
- Fixed size containers of items that are more efficient than Python `Lists` or `Tuples` for data processing.
- They only store single `data type` (Mixed data type is stored as string)
- They can be `1D` or multidimensional.
- Array elements can be modified, but array `size` cannot change.

```python
import numpy as np

marks = [50, 55, 90, 99, 100]

marks_array = np.array(marks)
```

### Key `Properties`

Properties | Description
:--- | :---
**ndim** | Number of dimensions (axes) in an array.
**shape** | Size of an array for each dimension.
**size** | Total number of elements in the array.
**dtype** | Data type of elements in the array.

<table>
  <tr>
    <th colspan="4"><h3>Dimensions ( Array )</h3></th>       
  <tr>
  <tr>
    <td colspan="4"><img src="Images/Dim.png" alt="Dimensions"></td>
  </tr>
  <tr>
    <td>0 Dimension</td>
    <td>1 Dimension</td>
    <td>2 Dimensions</td>
    <td>3 Dimensions</td>
  </tr>  
  <tr>
    <td>Point</td>
    <td>Line</td>
    <td>Square</td>
    <td>Cube</td>
  </tr>  
   <tr>
    <td>Scalar</td>
    <td>Vector ( Row or Column )</td>
    <td>Matrix ( Table or Data Frame )</td>
    <td>Tensor</td>
  </tr>  
  <tr>
    <td>Rank 0 Tensor</td>
    <td>Rank 1 Tensor</td>
    <td>Rank 2 Tensor</td>
    <td>Rank 3 Tensor</td>
  </tr>    
</table>

Array |	Dimensions
:--- | :---
`np.array([1, 2, 3])` |	`1D` Array
`np.array([(1, 2, 3), (4, 5, 6)])` | `2D` Array
`np.arange(start, stop, step)` | `Range` Array

Attribute | Description
:--- | :---
`ndarray.shape` | Tuple of array dimensions
`ndarray.size` | Number of elements present in the array
`ndarray.ndim` | Number of array dimensions ( 1, 2, 3 )
`ndarray.dtype` | Data type of Numpy array
`ndarray.itemsize` | Number of bytes required by each array element
`ndarray.nbytes` | Total number of bytes occupied by array
`ndarray.T` | NumPy.Transpose ( Transpose of a matrix )

Method | Description
:--- | :---
`array()` | Creates an array
`.arange()` | Creates an array in a range with a specified increment
`.unique()` | Number of unique elements in an array
`.repeat()` | Creates an array by repeating the number of elements  
`.argmax()` | Indices of maximum values along an axis
`.argmin()` | Indices of minimum values along an axis
`.reshape()` | Changes the shape of an array
`.count_nonzero()` | Count of non-zero elements in an array
`.hsplit()` | Split arrays horizontally ( Row wise )
`.vsplit()` | Split arrays vertically ( Column wise )
`.hstack()` | Stack arrays horizontally ( Row wise ) 
`.vstack()` | Stack arrays vertically ( Column wise )
`.flatten()` | Transform a multi-dimensional Numpy array to 1D Numpy array
`.ravel()` | View a multi-dimensional Numpy array as 1D Numpy array
`.transpose()` | Transposes an array
`np.absolute()` | Absolute values of elements in an array
`np.round()` | Round up the floats to a specified number of decimal points

[...](https://towardsdatascience.com/21-numpy-functions-that-will-boost-your-data-analysis-process-1671fb35215)

### Placeholders 

Operator | Description
:--- | :---
`np.linspace(0,2,9)` |	Add evenly spaced values between interval to array of length.
`np.zeros((1,2))`	| Creates an array filled with `zeros`
`np.ones((1,2))` |	Creates an array filled with `ones`
`np.random.random((5,5))` |	Creates an array with `random` numbers.
`np.empty((2,2))` |	Creates an `empty` array.

### `Similarities` between `Python Lists` and `NumPy Arrays`

- Both `lists` and `arrays` have similar syntax. 
- Elements in both are `ordered`, `mutable` and accept `duplicates`
- Both allows `indexing`, `slicing` and `iterating`

```python
# Python List
marks = [50, 45, 34]  

# NumPy Array
marks = np.array([50, 45, 34])
```

### `Differences` between `Python Lists` Vs `NumPy Arrays`

**Python List** | **NumPy Array**
:--- | :---
No support for vectorized operations | Support vectorized operations ( addition, multiplication )
Hold **Heterogeneous** / mixed data types | Hold **Homogeneous** data type
For loops are not efficient | For loops are fast and efficient
List is a default structure | Array needs import of NumPy library
Lists are flexible | Once the dimensions are defined cannot be expanded
Consumes more memory | Consumes 6x less memory
Slow ( Data type of each element is checked ) | Faster ( All the elements are of same data type )

Python List ( Ordered, Subscriptable, Mutable, Heterogeneous, Duplicate, Indexing, Slicing, Iterable )
```python
List = [1, 2, 3]
```

NumPy Array
```python
import numpy as np

Array = np.array([1, 2, 3])
```

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
