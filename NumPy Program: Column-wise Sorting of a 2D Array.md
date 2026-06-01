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
```python3
import os
os.environ["OMP_NUM_THREADS"]="1"
import numpy as np
a=eval(input())
arr=np.array(a)
print(arr)
print()
print(np.sort(arr,axis=0))

```

## Output
<img width="1541" height="725" alt="image" src="https://github.com/user-attachments/assets/6c3cfdfc-2851-4995-ad50-b155ad2d7202" />

## Result
Thus the program  that sorts the elements in each column of a given 2D array in ascending order is completed successfully.
