# NumPy Program: Column-wise Sorting of a 2D Array

## 🎯 Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

## 🧠 Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## 🧾 Program
Add code here
```
import numpy as np
rows = int(input("Enter number of rows: "))
cols = int(input("Enter number of columns: "))
print("Enter the elements row by row:")
elements = []
for i in range(rows):
    row = list(map(int, input(f"Row {i+1}: ").split()))
    elements.append(row)
array = np.array(elements)
sorted_array = np.sort(array, axis=0)
print("\nOriginal Array:\n", array)
print("\nColumn-wise Sorted Array:\n", sorted_array)
```
## Output
![Screenshot 2025-04-30 210443](https://github.com/user-attachments/assets/e9a43f60-1299-426b-a0aa-90317d7edcc7)
## Result
The code executed successfully.
