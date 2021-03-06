# VECTROISATION_ANALYSIS

## This doc gives the vectorisation computation compared to looping computation with time analysis comparision.

### Problem Statement: To compute square of a matrix (1-D, 2-D and 3-D). 

**Starting with 1-D computation**

Let the array be [11,21,31,41,51,61,71,81,91]

**Looping Construct**

```
temp = np.array([11,21,31,41,51,61,71,81,91])
res = []
for i in range(temp.shape[0]):
    res.append(temp[i]*temp[i])
```

**Vectorising**

The same operation can be done by translating the (column vector) to (row vector) and performing multiplication gives the square of a matrix.

<a href="https://www.codecogs.com/eqnedit.php?latex=A.A^{T}&space;=&space;A^{2}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?A.A^{T}&space;=&space;A^{2}" title="A.A^{T} = A^{2}" /></a>

Original Array

<a href="https://www.codecogs.com/eqnedit.php?latex=temp&space;=&space;[11,21,31,41,51,61,71,81,91]" target="_blank"><img src="https://latex.codecogs.com/gif.latex?temp&space;=&space;[11,21,31,41,51,61,71,81,91]" title="temp = [11,21,31,41,51,61,71,81,91]" /></a>

Transpose of Array

![](https://github.com/varunkodathala/Vectorisation_Analysis/blob/main/Square%20of%20Matrix/images/temp_transpose.png)

Square of Array

![](https://github.com/varunkodathala/Vectorisation_Analysis/blob/main/Square%20of%20Matrix/images/multiplication.png)


