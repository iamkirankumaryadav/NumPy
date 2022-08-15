# `Attribute`

```python
import numpy as np

x = np.array([1, 2, 3])

y = np.array([[1, 2, 3], [4, 5, 6]])

z = np.array([[[1,2,3], [4,5,6]], [[7,8,9], [10,11,12]]])

print(x)
print(y)
print(z)
```
 `output`
```
[1 2 3]

[[1 2 3]
 [4 5 6]]
 
[[[ 1  2  3]
  [ 4  5  6]]

 [[ 7  8  9]
  [10 11 12]]]
```

### `ndarray.shape`

```python
print(x.shape)
print(y.shape)
print(z.shape)
```
`output`
```
(3,)

(2, 3)

(2, 2, 3)
```

### `ndarray.ndim`

```python
print(f'Number of dimensions in x: {x.ndim}')
print(f'Number of dimensions in y: {y.ndim}')
print(f'Number of dimensions in z: {z.ndim}')
```
`output`
```
Number of dimensions in x: 1
Number of dimensions in y: 2
Number of dimensions in z: 3
```

### `ndarray.size`

```python
print(f'Number of elements in x: {x.size}')
print(f'Number of elements in y: {y.size}')
print(f'Number of elements in z: {z.size}')
```
`output`
```
Number of elements in x: 3
Number of elements in y: 6
Number of elements in z: 12
```
