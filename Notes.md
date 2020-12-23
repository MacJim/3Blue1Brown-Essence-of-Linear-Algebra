# 3Blue1Brown Essence of Linear Algebra Lecture Notes

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
