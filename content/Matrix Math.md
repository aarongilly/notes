---
aliases:
  - cross product
  - dot product
  - determinant
created: 2023-08-14T15:20-05:00
updated: 2024-01-01T23:13-06:00
---
**A graphical review of [[Matrices|Matrix]] operations**

Dot and cross products are still confusing. 

![[Pasted image 20240107120531.png]]
## Addition & Subtraction
Just add or subtract each element in `a` with its corresponding position in `b`.
## Magnitude
Use the Pythagorean theorem. Square all the terms, add them, then do a square root.


## 2x1 and 2x2
A vector on a 2d plane is defined by a vector `(a, b)`. If you take a 2x1 vector (or 1x2, doesn't matter) and multiply it by a 2x2 matrix, the result will be a new 2x1 vector, which is effectively just a *scaling and rotation* of the first one.

## Dot Product
The product of the magnitudes of the two vectors and the cosine of the angle between them. Not sure (yet) why this is an important operation.

Dot product yields a [[Matrix, Vector, Scalar|scalar]].

## Cross Product
The product of the magnitudes of the two vectors and the sine of the angle between them, times the unit vector that is normal to each of them. Again not sure (yet) why this is an important operation.

Cross Product yields a [[Matrices|Matrix]] with the same [[Cardinality]]. 

## Determinant
For a matrix to have a determinant, it must be a square (have an equal number of rows and columns). For a 2x2 matrix, the determinant is:
$$det\begin{pmatrix}
a & b \\ c & d
\end{pmatrix}=ad-bc
$$
Geometrically, the determinant tells you **the area of the parallelogram whose sides are defined by the matrix**. So, the parallelogram for the example above would have points (0,0), (a,b), (a+c,b+d),and (c,d) would have an area of `ad-bc`.

---
### Source
- Various websites, none of which were super helpful and thus aren't getting linked

### Related
- [[Matrix, Vector, Scalar]]
- [[Matrices|Matrix]]

#### Tags
#math 