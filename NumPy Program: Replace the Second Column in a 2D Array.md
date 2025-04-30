# NumPy Program: Replace the Second Column in a 2D Array

## 🎯 Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

## 🧠 Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

## 🧾 Program
Add code here
```
rows = int(input("Enter number of rows: "))
cols = int(input("Enter number of columns: "))
print("Enter the elements row by row:")
data = []
for i in range(rows):
    row = list(map(int, input(f"Row {i+1}: ").split()))
    data.append(row)
array = np.array(data)
print("\nEnter the new column values:")
new_col = []
for i in range(rows):
    val = int(input(f"Value for row {i+1}: "))
    new_col.append(val)
new_col = np.array(new_col).reshape(rows, 1)
array_without_col = np.delete(array, 1, axis=1)
updated_array = np.insert(array_without_col, 1, new_col, axis=1)
print("\nOriginal Array:\n", array)
print("\nUpdated Array (with replaced column):\n", updated_array)
```
## Output
![Screenshot 2025-04-30 211204](https://github.com/user-attachments/assets/2543bd8a-a6de-4ad7-a2d5-69d03d03327d)
## Result
The code executed successfully.
