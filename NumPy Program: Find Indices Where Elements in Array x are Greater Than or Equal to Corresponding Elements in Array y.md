# # NumPy Program: Find Indices Where Elements in Array x are Greater Than or Equal to Corresponding Elements in Array y

## 🎯 Aim
To write a Python program using **NumPy** that finds the indices where elements in array `x` are greater than or equal to their corresponding elements in array `y`.

## 🧠 Algorithm
1. **Import NumPy**: Import the NumPy library.
2. **Define Arrays**: Define two NumPy arrays, `x` and `y`, with the same shape (i.e., same number of elements).
3. **Use Boolean Indexing**: 
   - `x > y` gives a boolean array where elements of `x` are greater than `y`.
   - `x == y` gives a boolean array where elements of `x` are equal to `y`.
4. **Find Indices**: Use `np.where()` to get the indices where the conditions `x >= y` are satisfied.
5. **Print Indices**: Print the indices where the condition holds true.

## 🧾 Program
Add code here
```
import numpy as np
x = np.array([5, 3, 9, 1, 7])
y = np.array([2, 3, 4, 6, 7])
greater = x > y
equal = x == y
indices = np.where(x >= y)
print("Array x:", x)
print("Array y:", y)
print("x > y:", greater)
print("x == y:", equal)
print("Indices where x >= y:", indices[0]) 
```
## Output
![Screenshot 2025-04-30 210734](https://github.com/user-attachments/assets/11b1df91-967d-4557-8af5-79a1b8d48f4d)
## Result
The code executed successfully.
