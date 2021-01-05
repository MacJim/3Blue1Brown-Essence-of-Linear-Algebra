# 3Blue1Brown Essence of Linear Algebra Lecture Notes

- [3Blue1Brown Essence of Linear Algebra Lecture Notes](#3blue1brown-essence-of-linear-algebra-lecture-notes)
    - [3](#3)
    - [4](#4)
    - [5](#5)
    - [6](#6)
        - [Right Hand Axes](#right-hand-axes)
        - [Determinant Calculation](#determinant-calculation)
    - [7 Inverse Matrices, Column Space and Null Space uQhTuRlWMxw](#7-inverse-matrices-column-space-and-null-space-uqhturlwmxw)
    - [8 Nonsquare Matrices as Transformations Between Dimensions](#8-nonsquare-matrices-as-transformations-between-dimensions)
    - [9 Dot Products and Duality](#9-dot-products-and-duality)

Playlist: <https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab>

## 3

Source: <https://www.youtube.com/watch?v=kYB8IZa5AuE>

**Linear transformation** in layman's terms: after a linear transformation, lines remain lines, and the origin stays fixed.
In other words, keep grid lines parallel and evenly spaced.

Linear transformation in formulae:

![Linear Transformation Limits](3_files/linear_transformation_formulae.jpg)

## 4

**Composition** of multiple transformations `A @ B @ P`:

- Matrix multiplication of those individual transformation matrices
- The transformation of the rightward matrix `B` get applied first

## 5

Again, 3D transformation matrix's columns: new locations of the new unit vectors.

## 6

**Determinant** of a transformation: area (2D)/volume (3D) scaling factor.

Area scaling factor can be calculated by using square (0, 0, 1, 1):

- All squares have the same scaling factor
- Any area can be *approximated* by small enough squares

Values:

- 0 determinant ->
    - **reduce dimension**
    - Columns are linearly dependent
- Negative determinant -> "invert"/"flip" space

`det(AB) = det(A)det(B)`

### Right Hand Axes

![Right Hand Axes](6_files/right_hand_axes.png)

Can no longer use right hand axes after the transformation: determinant < 0

### Determinant Calculation

![2x2 matrix](6_files/determinant_2_2.png)

![3x3 matrix](6_files/determinant_3_3.png)

## 7 Inverse Matrices, Column Space and Null Space uQhTuRlWMxw

![Linear System of Equations](7_files/linear_system_of_equations.jpg)

![Linear System of Equations to Matrix Multiplication](7_files/linear_system_of_equations_to_matrix_multiplication.jpg)

Identity transformation: `inverse(A) @ A == I`

![Solve variables](7_files/solve_x.jpg)

`det(A) == 0`: Not inversible.
Solutions don't exist if the 2 equations contradict:

![Determinant 0 Solutions](7_files/det_0_solutions.jpg)

Rank: New dimensionality.
"full rank"

**Null space**/**kernel**: The set of vectors that lands on the origin after the transformation.
Describes solutions of `A @ x == [[0], [0]]`.

## 8 Nonsquare Matrices as Transformations Between Dimensions

![2D to 3D space](8_files/2d_to_3d_space.jpg)

Example: 2D vector to 3D vector

Column space: a plane in 3D space

![Column space](8_files/columns.jpg)

## 9 Dot Products and Duality

Dot product calculation using numbers:

![Basic Method](9_files/basic_method.jpg)

Dot product calculation using projection: `len(w's projection on v) * len(v)`

![Projection and Multiplication](9_files/projection_and_multiplication.jpg)

- If `w`'s projection is opposite to `v`, the dot product is negative
- Perpendicular vector: dot product is 0

Dot product usage: check if 2 vectors point in roughly the same direction.

`v . w == w . v`

Consider one of the vectors as a transformation matrix:

![Transformation](9_files/vector_and_transformation.jpg)

**Duality**: natural by surprising correspondence between 2 things.
