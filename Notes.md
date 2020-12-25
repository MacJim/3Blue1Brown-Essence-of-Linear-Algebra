# 3Blue1Brown Essence of Linear Algebra Lecture Notes

- [3Blue1Brown Essence of Linear Algebra Lecture Notes](#3blue1brown-essence-of-linear-algebra-lecture-notes)
    - [3](#3)
    - [4](#4)
    - [5](#5)
    - [6](#6)
        - [Right Hand Axes](#right-hand-axes)
        - [Determinant Calculation](#determinant-calculation)
    - [7 Inverse Matrices, Column Space and Null Space uQhTuRlWMxw](#7-inverse-matrices-column-space-and-null-space-uqhturlwmxw)

Playlist: <https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab>

## 3

Source: <https://www.youtube.com/watch?v=kYB8IZa5AuE>

**Linear transformation**: after a linear transformation, lines remain lines, and the origin stays fixed.
In other words, keep grid lines parallel and evenly spaced.

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

Can no longer use right hand axes after the transformation -> determinant < 0

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
