
#  EX 1 : NumPy Program: Column-wise Sorting of a 2D Array

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



<br>
<br>

#  EX 2:  NumPy Program: Find Indices Where Elements in Array x are Greater Than or Equal to Corresponding Elements in Array y

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
```python3
import os
os.environ["OMP_NUM_THREADS"]="1"

import numpy as np
x=np.array(eval(input()))
y=np.array(eval(input()))

print(np.where(x>y))
print(np.where(x==y))
```

## Output
<img width="1419" height="932" alt="image" src="https://github.com/user-attachments/assets/95c57f87-323d-45be-a5c4-1d0ed4893496" />

## Result
Thus the Python program using **NumPy** that finds the indices where elements in array `x` are greater than or equal to their corresponding elements in array `y` is completed successfully.

<br>
<br>




#  EX 3: Python Program to Perform Addition and Subtraction on Two NumPy Arrays

## 🎯 Aim
To write a Python program that performs addition and subtraction operations on two NumPy arrays.

## 🧠 Algorithm
1. Import the `numpy` library.  
2. Read two arrays from the user using `eval(input())`.  
3. Convert the inputs into NumPy arrays using `np.array()`.  
4. Perform addition using `arr1 + arr2`.  
5. Perform subtraction using `arr1 - arr2`.  
6. Print the results.  

## 🧾 Program
```python
import os
os.environ["OMP_NUM_THREADS"] = "1"
import numpy as np

arr1 = np.array(eval(input("Enter first array: ")))
arr2 = np.array(eval(input("Enter second array: ")))

print("Addition:\n", arr1 + arr2)
print()
print("Subtraction:\n", arr1 - arr2)
```

## 🖥️ Example Output

<img width="1425" height="915" alt="image" src="https://github.com/user-attachments/assets/f9ae734b-76b7-4a76-a614-ebe79584d9d4" />


## ✅ Result
Thus, the program has been successfully executed to perform addition and subtraction on two NumPy arrays.






<br>
<br>


#  EX 4: Python Program to Create Quarterly Sales DataFrame and Group by Category

## 🎯 Aim
To write a Python program that creates a DataFrame of quarterly sales, where each row contains the item category, item name, and expenditure. Then group the rows by category and print the total expenditure per category.

## 🧠 Algorithm
1. Import the `pandas` library.  
2. Read the sales data and column names from the user.  
3. Create a DataFrame using `pd.DataFrame(data, columns=col)`.  
4. Group the DataFrame by the `itemcat` column using `.groupby()`.  
5. Compute the sum of expenditures for each category using `.sum()`.  
6. Print the original DataFrame and the grouped result.  

## 🧾 Program
```python
import os
os.environ["OMP_NUM_THREADS"] = "1"
import pandas as pd

data = eval(input("Enter sales data: "))
col = eval(input("Enter column names: "))

qrtsales = pd.DataFrame(data, columns=col)
print(qrtsales)

qs = qrtsales.groupby('itemcat')
print("Result after Filtering Dataframe")
print(qs['expenditure'].sum())
```

## 🖥️ Example Output
<img width="1529" height="906" alt="image" src="https://github.com/user-attachments/assets/8fbc60ac-b564-4577-babd-9b733236515f" />



## ✅ Result
Thus, the program has been successfully executed to create a quarterly sales DataFrame and group the rows by category to calculate total expenditure.





<br>
<br>



# EX 5: Pandas Program: Join Two DataFrames Along Columns

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along Columns** (column-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames column-wise.
5. **Display Result**: Print the new combined DataFrame.

---

## 💻 Program
```python3
import os
os.environ["OMP_NUM_THREADS"]="1"
import pandas as pd
s1=pd.DataFrame(eval(input()))
s2=pd.DataFrame(eval(input()))
print("Original DataFrames:")
print(s1)
print("-------------------------------------")
print(s2)
print()
data=pd.concat([s1,s2],axis=1)
print("Join the said two dataframes along columns:")
print(data)
```

## Output
<img width="1533" height="887" alt="image" src="https://github.com/user-attachments/assets/af483952-650d-43f9-b367-e5ea79289dd4" />

## Result
Thus the is Python program using Pandas to **join two DataFrames along Columns** (column-wise concatenation) and assign all data to a new DataFrame completed successfully.
